# 資通安全概論(三天課程)

## 第1單元 資通安全基本觀念
- [資安威脅趨勢](資安威脅趨勢.md)
- [資通安全目標: CIA](CIA.md)
- Security `Program`
  - [NIST CSF 安全架構](NIST_CSF.md)
  - [ISO 27001 ISMS架構(第2單元)](ISMS_ISO_27001.md)

## 第2單元 資通安全相關法規
- A.法規 
  - 行政院國家資通安全會報
  - 資通安全管理法與子法
    - [資通安全管理法(23條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?pcode=A0030297)  [怎麼考?](資通安全管理法_考題.md)
    - 六大子法
      - 1.[資通安全管理法施行細則(13條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?pcode=A0030303)  [怎麼考?](施行細則_考題.md)
      - 2.[資通安全責任等級分級辦法(12條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?pcode=A0030304)  [怎麼考?](分級辦法_考題.md)
        - 第 2 條 公務機關及特定非公務機關（以下簡稱各機關）之資通安全責任等級，由高至低，分為 A 級、B 級、C 級、D 級及 E 級。
        - 附表1-8:應辦事項
        - 附表九 資通系統防護需求分級原則
        - 附表十 資通系統防護基準
      - 3.[資通安全事件通報及應變辦法(21條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?pcode=A0030305)
      - 4.[資通安全情資分享辦法(11條)](https://law.moj.gov.tw/lawclass/lawall.aspx?pcode=a0030307)
      - 5.[特定非公務機關資通安全維護計畫實施情形稽核辦法(10條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?media=print&pcode=A0030306)
      - 6.[公務機關所屬人員資通安全事項獎懲辦法(7條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?pcode=A0030308)
    - [資安法常見問題](https://moda.gov.tw/ACS/laws/faq/28/646)
      - 納管對象及範圍
      - 資通安全責任等級分級
      - 資通安全責任等級分級之應辦事項-資安專職人力及證照
      - 資通安全責任等級分級應辦事項-其他
      - 資通安全維護計畫撰寫及實施情形填報
      - 辦理受託業務-受託者之選任及監督
    - [國家機密保護法(41條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?PCode=I0060003)
    - [個人資料保護法(56條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?pcode=I0050021)
- B.[資訊安全管理系統 Information security management systems](ISMS_ISO_27001.md)


## 第3單元 資通安全風險管理與業務持續運作管理
- [風險管理](風險管理.md)
  - 【共通規範】| 資通系統風險評鑑參考指引(修訂)v4.1_1101231 
- [業務持續運作管理](業務持續運作管理.md)
  - 【共通規範】| 營運持續管理參考指引v2.0_1111231 

## 第4單元 作業安全 | 營運安全 security operation
- 軟硬體維護
- 組態管理(Configuration Management)
  - 組態管理Configuration Management)
  - 組態`變更`管理(Configuration Change Management)
  - 政府組態基準導入  ==> [政府組態基準(Government Configuration Baseline|GCB)](https://www.nics.nat.gov.tw/GCB.htm?lang=zh)
  - 政府機關弱點通報機制 ==> [ 資通安全弱點通報系統(Vulnerability Analysis and Notice System| VANS)](https://www.nics.nat.gov.tw/Vans.htm?lang=zh)
- 監控與問題管理
  - 異常的監控
    - 1.可用性監控
    - 2.完整性監控
    - 3.入侵偵測監控
    - 4.異常管理流程(incident handling)
    - 5.問題管理流程(problem handling)
  - 問題管理(Problem management)
    - 問題管理 WHAT
      - Problem management is the process of identifying and managing the causes of incidents on an IT service.
      - It is a core component of `ITSM(資訊科技服務管理|IT Service Management|ITSM|IT服務管理)`frameworks.
      - ITSM模組
        - 事故管理（Incident Management，ITIM）
        - 問題管理（Problem Management，ITPM）
        - 組態管理（Configuration Management）
        - 變更管理（Change Management，ITCM）
        - 財務管理（Financial Management for IT Services，ITFM）
    - 與作業安全的關聯 ==> 三大目標
      - 1.降低問題在服務上的衝擊
      - 2.降低錯誤與失敗狀況至可接受的基準
      - 3.防止相同問題重覆發生
    - 問題管理流程(problem handling)
      - 1.定義問題`優先序`
      - 2.調查分析問題發生`根本原因(ROOT CAUSE)`、問題追蹤(Problem tracking)
        - [根本原因分析|root cause analysis|RCA](https://zh.wikipedia.org/zh-tw/%E6%A0%B9%E6%9C%AC%E5%8E%9F%E5%9B%A0%E5%88%86%E6%9E%90)
        - [Problem Tracking Software Market Analysis 2022 | Demonstrates A Spectacular Growth By 2031](https://www.taiwannews.com.tw/en/news/4545236) 
      - 3.解決方案測試與實作 
- 資料備份管理
- 媒體控管(media management)
  - 媒體控管-目的及工作
  - 媒體控管-標示(labelling)
  - 媒體控管-重用(reuse)
  - 媒體控管-安全丟棄(disposal)
 - 可攜式設備管理(Mobile device management|MDM)
   - 可攜式設備(Mobile device)
   - 可攜式設備-安全問題
   - 可攜式設備管理-政策(policy)| 存取控制(access controls) |稽核(logging)
   - 可攜式設備管理工具與技術-自動化安裝或啟用控管程式
   - 可攜式設備-稽核紀錄內容
 - 弱點掃描(Vulnerability Scanning) ==> 目的 |
   - [OWASP|Vulnerability Scanning Tools| Dynamic Application Security Testing (DAST)](https://owasp.org/www-community/Vulnerability_Scanning_Tools)
   - 系統弱點掃描 ==> Nessus Pro | Nexpose
   - 網頁弱點掃描 ==> Acunetix | HCL AppScan(原IBM Security AppScan) | Fortify WebInspect(原 HP WebInspect)
 - 滲透測試(Penetration Test)
 - 稽核作業(Logging)-稽核紀錄分析(log analysis)
   - 稽核紀錄(log| log record)
   - 稽核紀錄分析(log analysis): 目的 | 
   - 稽核紀錄的保護(log protection)
   - [NIST SP 800-92 Guide to Computer Security Log Management](https://csrc.nist.gov/publications/detail/sp/800-92/final)
 - 社交工程演練 ==> 防範社交工程攻擊
- CISSP| Domain 7. Security Operations
## 第5單元 資訊委外安全
- 【共通規範】| 政府資訊作業委外資安參考指引v6.5_1131231
- 計畫階段
- 招標階段
- 決標階段
- 履約管理階段
- 驗收階段
- 保固階段
## 第6單元 存取控制與加解密技術
- 【共通規範】| 身分鑑別與存取控制參考指引v2.0_1111231
- 存取控制
- 身分驗證 
- 密碼學加解密技術 
  - 密碼學的應用 [補充教材下載](./密碼學的應用.pdf) 
    - 密碼學的應用1:數位信封與數位簽章 [教學影片](https://youtu.be/LIG-mXyJTG0)
    - 密碼學的應用2:PKI 公開金鑰基礎建設[教學影片](https://youtu.be/G02vkzLSrE4)

## 第7單元 網路安全與實體安全
- 網路安全防禦技術
  - 防火牆 == > 【共通規範】| 防火牆建置資安參考指引(修訂)v3.0_1091015
  - 入侵偵測與防禦系統 == > 【共通規範】| 入侵偵測與防禦系統建置資安參考指引(修訂)v2.0_1091015 
  - 虛擬私有網路(VPN) == > 【共通規範】| VPN安全參考指引(修訂)v2.2_1101231
  - 防毒系統
  - 垃圾郵件過濾系統  == > 【共通規範】| 電子郵件安全參考指引(修訂)v3.1_1101231
  - 端點偵測及回應系統(EDR)
  - SOC(本教材沒有) == > 【共通規範】| 領域SOC實務建置指引v1.0_1060301
- 網路區域規劃 == >  【共通規範】| 網路架構規劃參考指引(修訂)v3.1_1101231
- 網路連線安全 == > 
- 雲端運算安全 == > 【共通規範】| 政府機關雲端服務應用資安參考指引v1.3_1131231
- 實體安全 == > 

## 第8單元 應用程式安全
- 不安全的程式
  - 緩衝區溢位(Buffer overflow)
  - 惡意程式(Malware)
  - 邏輯炸彈(logical bomb)
  - 隱藏通道(Covert Channel)
  - 輸入攻擊
- 軟體開發生命週期安全(Secure Software Development Life Cycle, SSDLC)
- 應用程式安全控制==> 強化程式安全的各種做法
  - 變更控制(Change Controls)
  - 職責區隔(SOD|Segregation Of Duties)
  - 程式庫維護
  - 應用程式安全檢測
    - 入侵防禦系統(Intrusion Prevention System, IPS)：具備部份防禦功能
    - 源碼檢測(Static Code Analysis)：使用自動化的源碼檢測工具找出有問題的程式碼
      - ==> SAST（Static Application Security Testing，靜態應用程式安全測試）對應用程式原始碼執行直接的白盒分析(whitebox)
    - 網頁應用程式防火牆(Web Application Firewall, WAF)：針對應用層攻擊進行防禦
      - SEE  Gartner《Magic Quadrant for Web Application Firewalls》 [結果](https://www.bing.com/images/search?view=detailV2&ccid=YeX1%2fO0q&id=F2FDD2C854AE30D65E60F8213E310F81D4FC6F72&thid=OIP.YeX1_O0qsIzM2oLgmgUp3wHaHa&mediaurl=https%3a%2f%2fwww.detectx.com.au%2fwp-content%2fuploads%2f2018%2f10%2f340592_0001.png&cdnurl=https%3a%2f%2fth.bing.com%2fth%2fid%2fR.61e5f5fced2ab08cccda82e09a0529df%3frik%3dcm%252f81IEPMT4h%252bA%26pid%3dImgRaw%26r%3d0&exph=1393&expw=1393&q=Gartner+Magic+Quadrant+for+Web+Application+Firewalls&simid=608041158312734857&FORM=IRPRST&ck=6823EB0D2614C0480AEDB0D391F87354&selectedIndex=0&itb=1)
    - [Cloud Web Application and API Protection](https://www.gartner.com/reviews/market/cloud-web-application-and-api-protection)
    - 滲透測試(Penetration Test, PT )：模擬攻擊者行為找出網站漏洞 ==> 黑盒分析(blackbox)
    - 網站弱點評估(Web Vulnerability Assessment)：使用掃描工具檢測弱點
      - ==> DAST（dynamic Application Security Testing，動態應用程式安全測試） 
- 行動應用程式安全(Mobile app Security)
  - 政府行動化安全防護規劃報告V1.0」第61~62頁
  - 行動應用程式的開發過程，會衍生二大安全議題:
    - 1.行動應用程式碼的安全性議題 :
      - 因撰寫方式的錯誤，使用Apps存有安全弱點，導致系統遭入侵
      - 參考OWASP Mobile TOP 10
        - Top 10 Mobile Risks Beta 2 Draft 2023
      - 行動裝置資安防護參考指引
      - 解決方法建議遵守安全系統發展生命週期進行開發，藉助第三方或是自動化檢測進行白箱、黑箱靜態與動態之檢測。
        - [OWASP Mobile Application Security](https://owasp.org/www-project-mobile-app-security/)
        - [OWASP Mobile Application Security Verification Standard (MASVS)](https://owasp.org/www-project-mobile-app-security/)
        - [Mobile Application Security Checklist](https://owasp.org/www-project-mobile-app-security/)
    - 2.隱私侵犯的議題
      - 因程式開發時，索取過多行動裝置上的敏感資訊，例如：通訊錄、行事曆、座標位置、郵件、簡訊內容等
      - 建議遵守Privacy by Design之原則，將隱私保護之概念，融入於應用程式的設計 
- Web應用程式安全(Web app Security)
  - [OWASP Top 10 2021](https://owasp.org/Top10/zh_TW/)
  - A1	權限控制失效(Broken Access Control)
  - A2	加密機制失效(Cryptographic Failures)
  - A3	注入式攻擊(Injection)
    - SQL Injection
    - XSS (JAVAscript Injection)
    - Command Injection
    - LDAP Injection
    - .....
  - A4	不安全設計(Insecure Design)
  - A5	安全設定缺陷(Security Misconfiguration)
  - A6	危險或過舊的元件(Vulnerable and Outdated Components)
  - A7	認證及驗證機制失效(Identification and Authentication Failures)
  - A8	軟體及資料完整性失效(Software and Data Integrity Failures)
  - A9	資安記錄及監控失效(Security Logging and Monitoring Failures)
  - A10	伺服端請求偽造(Server-Side Request Forgery)
- Cloud NAtive-APP雲端原生應用程式
  - Cloud-native applications雲端原生應用程式
  - OWASP Cloud-Native Application Security Top 10(尚未定稿| 缺人)
- [Internet of Things (IoT) Top 10 2018](https://wiki.owasp.org/index.php/OWASP_Internet_of_Things_Project#tab=IoT_Top_10)
## 第9單元 資通安全健診
- 資通安全健診:目的
- 資通安全健診:項目
  - 機關定期辦理資通安全健診(A級機關每年1次，B級機關每2年1次)，檢測項目包含：
    - 1.網路架構檢視
    - 2.網路惡意活動檢視
      - a.封包側錄
      - b.資安設備紀錄檔(log)分析
    - 3.使用者端電腦惡意活動檢視
    - 4.伺服器主機惡意活動檢視
    - 5.目錄伺服器(Directory Service)設定檢視 ==> Windows Server 2022 AD(active Directory)的安全設定
    - 6.防火牆連線設定檢視 ==>防火牆規則檢視
- 資通安全健診:流程
- 
## 第10單元 資通安全事件通報及應變
- incident vs event
- [資通安全事件通報及應變辦法(共21條)](https://law.moj.gov.tw/LawClass/LawAll.aspx?pcode=A0030305)
  - 第一章 總則
    - 第 2 條 資通安全事件分為四級。
      - 資通安全事件分級由輕至重分「1」、「2」、「3」、「4」四個級別
      - 這四個級別怎麼定?
    - 第 3 條 資通安全事件之`通報內容`  ==> 參考3-63頁
  - 第二章 公務機關資通安全事件之通報及應變
    - 第 4 條 通報
    - 第 5 條 審核
    - 第 6 條 應變 ==>
    - 第 9 條 `通報`作業規範
    - 第 10 條 `應變`作業規範
 - 第三章 特定非公務機關資通安全事件之通報及應變
    - 第 11 條 通報
    - 第 12 條 審核
    - 第 13 條 應變 ==>
    - 第 15 條 `通報`作業規範
    - 第 15 條 `應變`作業規範
 - 第四章 附則
   - 第 18 條 公務機關 資通安全演練作業
   - 第 19 條  特定非公務機關  資通安全演練作業
- 資安事件處理(incidenet handling)
  - [NIST SP 800 61r2 Computer Security Incident Handling Guide ](https://nvlpubs.nist.gov/nistpubs/specialpublications/nist.sp.800-61r2.pdf)
  - 目的
  - 資安事件處理計畫
  - 資安事件處理程序|流程
    - 準備：資安事件處理時所需之專業人員、組織分工、處理與鑑識的訓練、計畫與程序的編撰及模擬演練
識別：當資安事件發生時，第一步驟是識別資安事件的嚴重性與影響範圍
封鎖：封鎖入侵來源，以避免災害擴大
根除：徹底清除被植入的惡意程式並修補被入侵的管道。
回復：被入侵的系統回復至正常運作的狀況
經驗學習：在事件中學習到相關的經驗，並反應在資安政策與防護措施上，以避免相同問題再度發生

 
  - NIST SP 800-53, Revision 5| IR: Incident Response   Controls [參考資料](https://csf.tools/reference/nist-sp-800-53/r5/ir/)
    - IR-1: Policy and Procedures
    - IR-2: Incident Response Training
    - IR-3: Incident Response Testing  ==> BASELINE(S):Moderate  High   Privacy
    - IR-4: Incident Handling
    - IR-6: Incident Reporting
    - IR-7: Incident Response Assistance
    - IR-8: Incident Response Plan
    - 電腦緊急應變小組（Computer Emergency Response Team，CERT）
    - 電腦資安事件應變小組（Computer Security Incident Response Team，CSIRT）
      - [CSIRT| ithome專刊](https://www.ithome.com.tw/taxonomy/term/13043/all)
    - 產品資安事件應變小組（Product Security Incident Response Team，PSIRT）

- [Incident Handling & Response Career Path(入侵處理與響應 資安職涯發展) | EC-Council](https://www.eccouncil.org/incident-handling-response-career-path/)
 
- 數位證據(Digital Evidence)

