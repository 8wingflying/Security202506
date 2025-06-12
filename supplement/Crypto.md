# Crypto
# 密碼學
- 古典密碼 ==> [凱薩密碼](https://en.wikipedia.org/wiki/Caesar_cipher)  | [密碼棒Scytale](https://en.wikipedia.org/wiki/Scytale)
- 現代密碼 ==> 安全性來自:數學難解 ==> 但可輕鬆被量子電腦秒殺
  - 對稱式 ==> DES | 3DES | AES
  - 非對稱式 ==>　RSA | Elgama
  - Hash(雜湊)
    - MD5
    - SHA1 
- 量子密碼 ==> 安全性來自量子力學的根本原理
- 後量子密碼 ==> 設計不會被量子電腦
  - 後量子密碼學| Post-quantum cryptography(PQC)，又稱為防量子、量子安全、抗量子計算，是密碼學的一個研究領域
  - 專門研究能夠抵抗`量子電腦`進行密碼分析攻擊的加密演算法（特別是公鑰加密演算法）
### RSA 非對稱式
##### 質因數因式分解
- 質因數因式分解有多難? 15 == 5*3 ??
  - https://zh.wikipedia.org/zh-tw/RSA%E5%8A%A0%E5%AF%86%E6%BC%94%E7%AE%97%E6%B3%95
  - 1999年，RSA-155（512 bits）被破
  - 2009年12月12日，編號為RSA-768（768 bits, 232 digits）數也被成功分解 

## 範例試題1
```
密碼學常被認為是提供數位身分認證的基礎，請問一套加密系統「不」 包含下列何者？
(A) 明文
(B) 暴力破解機制
(C) 加密演算法
(D) 密文
```
## 範例試題2
```
關於密碼學（Cryptography）所能達成之主要目的，下列何項錯誤？
(A) 機密性（confidentiality）
(B) 完整性（Integrity）
(C) 可用性（Availability）
(D) 不可否認性（Non-Repudiation）
```
## 範例試題3
```
下列何種機制「不」可用於加密及解密？
(A) AES Advanced Encryption Standard
(B) DES Data Encryption Standard
(C) RSA Rivest-Shamir-Adleman
(D) MD5 Message-Digest Algorithm 
```
## 範例試題4
```
下列何者「不」是對稱式加密（Symmetric Encryption）？
(A) 資料加密標準（Data Encryption Standard, DES）
(B) 三重資料加密演算法（Triple DES, 3DES）
(C) 橢圓曲線密碼學（Elliptic Curve Cryptography, ECC）
(D) RC6 加密演算法（Rivest Cipher 6, RC6）
```

## 範例試題5
```
下列何種加密技術，屬於「非對稱式金鑰加密技術」？
(A) 國際資料加密演算法（International Data Encryption Algorithm, IDEA）
(B) 進階加密標準（Advanced Encryption Standard, AES）
(C) 資料加密標準（Data Encryption Standard, DES）
(D) 橢圓曲線密碼學（Elliptic Curve Cryptography, ECC）
```
## 範例試題6
```
關於公鑰（Public Key）與私鑰（Private Key）加解密，下列敘述何者 「不」正確？
(A) 公私鑰加解密演算法使用「公鑰加密」與「私鑰解密」
(B) 數位簽章的時候，傳送端使用自己的公鑰製作簽章，接收端使用 傳送端的私鑰驗證簽章
(C) 公鑰加密系統是多人都可以拿公鑰加密，但是只有一個人可以拿 私鑰解密
(D) 數位簽章系統是只有一個人可以拿私鑰製作簽章，但是多人都可 以拿公鑰驗證簽章
```
## 範例試題7
```
關於非對稱式加密（Asymmetric Encryption），下列敘述何者「不」正 確？
(A) 非對稱式加密又稱公私鑰加密，顧名思義具有公鑰與私鑰，公鑰 可公開，私鑰則須妥善保管
(B) 傳送方於傳送時可利用私鑰進行加密，接收方利用公鑰則可驗證 檔案所有人
(C) 公鑰與私鑰為成對存在
(D) 若有 N 個使用者，則須 N+1 對金鑰（公鑰與私鑰為一對）
```
## 範例試題8
```
關於「對稱式金鑰加密」與「非對稱金鑰加密」，下列敘述何者「不」 正確？
(A) 「非對稱金鑰加密」在加解密使用不同金鑰
(B) 「對稱金鑰加密」在金鑰洩露後，其加密效果即時失效
(C) 「非對稱金鑰加密」的特性，可以實作數位簽章（Digital Signature）
(D) 「非對稱金鑰加密」的計算，效能比「對稱金鑰加密」佳
```
## 複選題_範例試題1
```
關於對稱式加密（Symmetric Encryption），下列敘述何者「不」正 確？
(A) 對稱式加密特色為加解密速度快，若使用長金鑰具備相對較高之 安全性
(B) 對稱式加密金鑰管理是重要的課題，若有 N 位使用者，則需 N×(N-1)金鑰數目
(C) 對稱式加密中，金鑰的管理極為重要，為決定安全性之根本之一
(D) 對稱式演算法可以驗證檔案所有人身分
```



# 應用 數位簽章（Digital Signature）及數位信封（Digital Envelop）
## 範例10
```
關於數位簽章（Digital Signature）及數位信封（Digital Envelop），下列敘述何者正確？
(A) 數位簽章與數位信箱皆運用雜湊函式（Hash Function）達成效果
(B) 數位簽章主要是將訊息摘要加密後運用對稱金鑰加密
(C) 數位信封將資料以對稱金鑰加密，再將金鑰透過公開金鑰加密技 術傳輸供收訊方解密
(D) 數位簽章及數位信封技術在訊息傳遞時皆已加密訊息
```
## 範例11
```
關於數位簽章（Digital Signature），下列敘述何者「不」正確？
(A) 使用了公開金鑰基礎建設（Public Key Infrastructure, PKI）
(B) 簽章時用公鑰（Public Key）加密
(C) 公鑰（Public key）必須向接受者信任的數位憑證認證機構 （Certificate Authority, CA）註冊
(D) 可以用 EIGamal 演算法來實做數位簽章
```




