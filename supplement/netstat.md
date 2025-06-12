# [netstat](https://learn.microsoft.com/zh-tw/windows-server/administration/windows-commands/netstat)
- Windows/Linux 用來查看網路連線、路由表、連接埠狀態及相關統計資訊的工具
- 常常被用來檢測網路環境是否正常，對於網管或相關領域的人員來說是一定要會的指令
- [使用 Netstat 指令檢測網路的技巧](https://blog.gtwang.org/linux/linux-netstat-command-examples/)
- [[Linux] netstat 查看網路狀態，指令範例教學](https://www.jinnsblog.com/2020/12/linux-netstat-network-status.html)
- 更多Windows commands 請參看 [Windows 命令 | Microsoft Learn](https://learn.microsoft.com/zh-tw/windows-server/administration/windows-commands/windows-commands)
## netstat /?  (netstat -help)
- 顯示通訊協定統計資料和目前的 TCP/IP 網路連線。
```
NETSTAT [-a] [-b] [-e] [-f] [-i] [-n] [-o] [-p proto] [-r] [-s] [-t] [-x] [-y] [interval]

 -a            顯示所有連線和接聽連接埠。
 -b            顯示建立每個連線或接聽連接埠時涉及的可執行檔。
               在某些情況下，已知的可執行檔承載多個獨立元件，在這些情況下，
               將顯示建立連接線時或接聽連接埠時涉及的元件順序。
               在此案例中，可執行檔名稱位於 [] 底部，最上方是它呼叫的元件，
               以此類推，直到達到 TCP/IP。
               請注意，這個選項可能會很耗時，而且會失敗，除非您有足夠的權限。
 -c            顯示按當前消耗的 TCP 或 UDP 連接埠排序的程序清單。
 -d            顯示與每個連線有關的 DSCP 值。
 -e            顯示乙太網路統計資料。這可與 -s 選項結合。
 -f            顯示適用於外部地址之完全合格的網域名稱 (FQDN)。
 -i            顯示 TCP 連線目前狀態所花費的時間。
 -n            以數位格式顯示位址和連接埠號碼。
 -o            顯示與每個連線相關聯的擁有處理識別碼。
 -p proto      顯示 proto 所指定通訊協議的連線;proto
               可能是下列任何一種: TCP、UDP、TCPv6 或 UDPv6。如果與 -s 選項
               一起使用以顯示每個通訊協定統計資料，proto 可能是下列任何一種:
               IP、IPv6、ICMP、ICMPv6、TCP、TCPv6、UDP 或 UDPv6。
 -q            顯示所有連線，接聽連接埠和繫結非接聽 TCP 連接埠。
               繫結的非接聽連接埠可能或可能不會與使用中的連線相關聯。
 -r            顯示路由表格。
 -s            顯示每個通訊協定統計資料的資訊。根據預設，會顯示
               顯示 IP、IPv6、ICMP、ICMPv6、TCP、TCPv6、UDP 和 UDPv6 的統計資訊;
               -p 選項可用來指定預設值的子集。
 -t            顯示目前的連線卸載狀態。
 -x            顯示 NetworkDirect 連線、聆聽程式及共用的端點。
 -y            顯示所有連線的 TCP 連線範本。
               無法與其他選項合併。
 間隔      在每個顯示之間重新顯示已選取的統計資料，
               其翁暫停間隔秒數。按 CTRL+C 可以停止重新顯示
               統計資料。如果省略，netstat 將會列印目前的
               設定資訊一次。
```

#### 範例考題
```
netstat是Windows/Linux台上用來顯示通訊協定統計資料和目前的 TCP/IP 網路連線的重要工具
底下為某資安專職人員在Windows 11執行netstat的畫面
請問你他使用的參數是哪一個?
(A) netstat -ano   (B)netstat -an    (C)netstat -anob  (D)netstat /?

使用中連線

  協定   本機位址               外部位址               狀態            PID
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING       1948   RpcSs [svchost.exe]
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING       4      無 法取得擁有權資訊
  TCP    0.0.0.0:623            0.0.0.0:0              LISTENING       5268   [LMS.exe]
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING       10600  CDPSvc [svchost.exe]
  TCP    0.0.0.0:5357           0.0.0.0:0              LISTENING       4       無法取得擁有權資訊
  TCP    0.0.0.0:6646           0.0.0.0:0              LISTENING       6120    [MMSSHOST.EXE]
  TCP    0.0.0.0:7680           0.0.0.0:0              LISTENING       24344   無法取得擁有權資訊
  TCP    0.0.0.0:16992          0.0.0.0:0              LISTENING       5268     [LMS.exe]
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING       1556     無法取得擁有權資訊
  ................................

```

```
(A) netstat -a  (B)netstat -an    (C)netstat -ano  (D)netstat /?

使用中連線

  協定   本機位址               外部位址               狀態
  TCP    0.0.0.0:135            DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:445            DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:623            DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:5040           DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:5357           DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:6646           DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:7680           DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:16992          DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:49664          DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:49665          DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:49666          DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:49669          DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:49670          DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:49717          DESKTOP-A8AERON:0      LISTENING
  TCP    0.0.0.0:55168          DESKTOP-A8AERON:0      LISTENING
  TCP    127.0.0.1:9656         DESKTOP-A8AERON:0      LISTENING
  TCP    127.0.0.1:24830        DESKTOP-A8AERON:0      LISTENING
  TCP    127.0.0.1:41343        DESKTOP-A8AERON:0      LISTENING
  TCP    127.0.0.1:49677        DESKTOP-A8AERON:49678  ESTABLISHED
  TCP    127.0.0.1:49678        DESKTOP-A8AERON:49677  ESTABLISHED
```

```
下圖為A級某資安專職人員執行 netstat的畫面
請問你他使用底下哪一個參數?
(A) netstat -a  (B)netstat -an    (C)netstat -ao  (D)netstat /?


使用中連線

  協定   本機位址               外部位址               狀態            PID
  TCP    0.0.0.0:135            DESKTOP-A8AERON:0      LISTENING       1948
  TCP    0.0.0.0:445            DESKTOP-A8AERON:0      LISTENING       4
  TCP    0.0.0.0:623            DESKTOP-A8AERON:0      LISTENING       5268
  TCP    0.0.0.0:5040           DESKTOP-A8AERON:0      LISTENING       10600
  TCP    0.0.0.0:5357           DESKTOP-A8AERON:0      LISTENING       4
  TCP    0.0.0.0:6646           DESKTOP-A8AERON:0      LISTENING       6120
  TCP    0.0.0.0:7680           DESKTOP-A8AERON:0      LISTENING       24344
  TCP    0.0.0.0:16992          DESKTOP-A8AERON:0      LISTENING       5268
  TCP    0.0.0.0:49664          DESKTOP-A8AERON:0      LISTENING       1556
  TCP    0.0.0.0:49665          DESKTOP-A8AERON:0      LISTENING       1472
  TCP    0.0.0.0:49666          DESKTOP-A8AERON:0      LISTENING       2640
  TCP    0.0.0.0:49669          DESKTOP-A8AERON:0      LISTENING       2424
  TCP    0.0.0.0:49670          DESKTOP-A8AERON:0      LISTENING       3964
  TCP    0.0.0.0:49717          DESKTOP-A8AERON:0      LISTENING       1548
  TCP    0.0.0.0:55168          DESKTOP-A8AERON:0      LISTENING       24068
  TCP    127.0.0.1:9656         DESKTOP-A8AERON:0      LISTENING       10620
  TCP    127.0.0.1:24830        DESKTOP-A8AERON:0      LISTENING       4740
  TCP    127.0.0.1:41343        DESKTOP-A8AERON:0      LISTENING       14852
```
