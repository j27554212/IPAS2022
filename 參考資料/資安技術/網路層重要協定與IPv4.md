# 網路層重要協定

- [ARP 與 RARP 協定](http://www.tsnien.idv.tw/Internet_WebBook/chap5/5-3%20ARP%20%e8%88%87%20RARP%20%e9%80%9a%e8%a8%8a%e5%8d%94%e5%ae%9a.html)
- [ICMP 協定](http://www.tsnien.idv.tw/Internet_WebBook/chap5/5-4%20ICMP%20%e9%80%9a%e8%a8%8a%e5%8d%94%e5%ae%9a.html)
- [IGMP 協定](http://www.tsnien.idv.tw/Internet_WebBook/chap5/5-5%20IGMP%20%e9%80%9a%e8%a8%8a%e5%8d%94%e5%ae%9a.html)
- [IPv6 協定](http://www.tsnien.idv.tw/Internet_WebBook/chap5/5-6%20IPv6%20%e9%80%9a%e8%a8%8a%e5%8d%94%e5%ae%9a.html)

- [第六章 IP Routing 協定](http://www.tsnien.idv.tw/Internet_WebBook/chap6/6-0%20%e7%bf%92%e9%a1%8c.html)

## IP FORMAT [IP 封包結構](http://www.tsnien.idv.tw/Internet_WebBook/chap5/5-2%20IP%20%e9%80%9a%e8%a8%8a%e5%8d%94%e5%ae%9a.html)

```
● 版本（Version）：4 位元。表示 IP 封包的 IP 版本。

● 網際標頭長度（Internet Header Length, IHL）：4 位元。表示本 IP 封包標頭的長度（位元組表示）。範圍為 5 ~ 15，預設值為 5。

● 服務型態（Type of Service, TOS）：8 位元。其內容為 "PPPDTRUU"，PPP 表示本 IP 封包的優先權（Precedence）；D = 0 表示一般延遲（Delay），D = 1 表示低延遲；T = 0 為一般傳送量（Throughput），T = 1 為高傳送量；R = 0 為一般可靠度，R = 1 為高可靠度（Reliability）；UU 保留未用。

● 總長度（Total Length）：16 位元。是指該封包的總長度，包括封包標頭及資料的長度，範圍由 576 ~ 65535 位元組。

● 辨識碼（Identification）：8 位元。表示資料分割（fragmentation）的識別編號。同一筆資料如被分割成若干個區段，每段給予相同的辨識碼，接收端再依辨識碼組合回原來資料封包。

● 旗標（Flags）：3 位元。其格式為 "0DM"。D = 0 表示可以分段，D = 1 為不可分段（Don’t fragment）；M = 0 表示最後分段，M = 1 為不是最後分段（More fragment）。

● 分段偏移（Fragment Offset）：13 位元。表示目前的分段在原始的資料中所在的位址。原始分段允許有 8192 個分段，以每 8 個位元為一個基本偏移量，所以最大容許 65536 位元資料，此值和總長度一樣。因此範圍為 0 ~ 8191，預設值為 0。

● 存活時間（Time to Live, TTL）：8 位元。表示該封包在網路上的存活時間，封包每經過一個路由器（或網路閘門），該值就被減一。如路由器發現某封包的 TTL = 0，便將該資料片丟棄而不轉送。範圍 0 ~ 255。

● 協定號碼（Protocol Number）：8 位元。表示該 IP 封包所承載通訊協定的協定號碼。在 TCP/IP 協定中，任何通訊協定（如IP、ICMP、TCP、UDP等等）的資料在傳送中都被包裝成 IP 封包，而以 IP 通訊協定發送。所以，在IP 封包裡必須有協定號碼欄位，來表示目前所承載之資料是屬於哪一個通訊協定（IP、ICMP、TCP 等等）。一些較常用著名（well-known）的協定號碼如表 5-1 所示。

● 標頭檢查集（Header Checksum）：16 位元。做標頭錯誤檢查用。

● 來源位址（Source Address）：32 位元。發送此 IP 封包的來源位址。

● 目的位址（Destination Address）：32 位元。目的主機之位址。

● 選項欄位（Options）：可變長度。提供多種選擇性服務。目前已定義使用有下列：

(1) 安全處理機制：有關資料加密與認證。

(2) 路由紀錄：當 IP 封包經過路由器時，讓該路由器登錄其 IP 位址。當封包到達目的地時，可追蹤它所經過的路徑。

(3) 時間戳記：當 IP 封包經過路由器時，讓路由器登錄其 IP 位址和時間。

(4) 寬鬆來源路由（Loose Source Routing）：記錄該封包所必須經由之路徑，為一 IP 位址的序列表。

(5) 嚴格來源路由（Strict Source Routing）：如同寬鬆來源路由，但嚴格規定祇能依照 IP 序列表傳送該封包。

● 填補欄位（Padding）：IP 資料片的標頭一定是 32 位元的整數倍，當 Options 欄位不足 32 位元整數倍時由 Padding 欄位補足。
```
