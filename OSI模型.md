# [OSI模型 ( 開放式系統互聯模型 )](https://zh.wikipedia.org/wiki/OSI%E6%A8%A1%E5%9E%8B)
OSI模型(Open Systems Interconnection Reference Model)國際標準化組織提出，一個試圖使各種電腦在世界範圍內互連為網路的標準框架。\
該模型將通訊系統中的資料流`劃分為七個層`，從分散式應用程式資料的最高層表示到跨通訊媒介傳輸資料的物理實現。每個中間層為其上一層提供功能，其自身功能則由其下一層提供。功能的類別通過標準
的通訊協定在軟體中實現。
## 層次劃分
OSI將電腦網路體系結構劃分為七層。`( 第1層為底部，第七層為頂部 )`
|層級|名稱|功能|
|-|-|-|
|第7層|應用層(Application Layer)|提供為應用軟體而設計的介面，以設定與另一應用軟體之間的通訊。|
|第6層|表達層(Presentation Layer)|把數據轉換為能與接收者的系統格式相容並適合傳輸的格式。|
|第5層|會議層(Session Layer)|在數據傳輸中設定和維護電腦網路中兩台電腦之間的通訊連接。|
|第4層|傳輸層(Transport Layer)|將傳輸表頭加至數據以形成數據包。傳輸表頭包含了所使用的協定等傳送資訊。|
|第3層|網路層(Network Layer)|決定數據的路徑選擇和轉寄，將網路表頭加至數據包，以形成封包。網路表頭包含了網路資料。|
|第2層|資料連結層(Data Link Layer)|負責網路尋址、錯誤偵測和改錯。分為兩個子層：邏輯鏈路控制(LLC)層和媒介存取控制(MAC)層。|
|第1層|實體層(Physical Layer)|管理電腦通訊裝置和網路媒體之間的互通。|

![image](https://user-images.githubusercontent.com/91179289/138015084-101929eb-40ff-4ee2-a5e7-92b613cd7892.png)
|OSI model|||
|-|-|-|
|L7 應用層(Application Layer)||[L7-Switch交換器](https://github.com/Ruass1970E/4100E022/blob/main/OSI%E6%A8%A1%E5%9E%8B.md#l7-switch)|
|L6 表達層(Presentation Layer)|||
|L5 會議層(Session Layer)|||
|L4 傳輸層(Transport Layer)||[L4-Switch交換器](https://github.com/Ruass1970E/4100E022/blob/main/OSI%E6%A8%A1%E5%9E%8B.md#l4-switch)|
|L3 網路層(Network Layer)|[路由器 Router](https://github.com/Ruass1970E/4100E022/blob/main/OSI%E6%A8%A1%E5%9E%8B.md#%E8%B7%AF%E7%94%B1%E5%99%A8router)|[L3-Switch交換器](https://github.com/Ruass1970E/4100E022/blob/main/OSI%E6%A8%A1%E5%9E%8B.md#l3-switch)|
|L2 資料連結層(Data Link Layer)||[L2-Switch交換器](https://github.com/Ruass1970E/4100E022/blob/main/OSI%E6%A8%A1%E5%9E%8B.md#l2-switch)|
|L1 實體層(Physical Layer)|[中繼器 Repeater](https://github.com/Ruass1970E/4100E022/blob/main/OSI%E6%A8%A1%E5%9E%8B.md#%E4%B8%AD%E7%B9%BC%E5%99%A8repeater)|[集線器 HUB](https://github.com/Ruass1970E/4100E022/blob/main/OSI%E6%A8%A1%E5%9E%8B.md#%E9%9B%86%E7%B7%9A%E5%99%A8hub)|
## [路由器(Router)](https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E5%99%A8)
指一種電訊網路裝置，提供路由與轉送兩種重要機制，
可以決定封包從來源端到目的端所經過的路徑（host到host之間的傳輸路徑），
這個過程稱為路由；將路由器輸入端的封包移送至適當的路由器輸出端（在路由器內
部進行），這稱為轉送。路由工作在OSI模型的第三層，即網路層，例如網際協定（IP）。\
(https://zh.wikipedia.org/wiki/%E8%B7%AF%E7%94%B1%E5%99%A8)
## [中繼器(Repeater)](https://zh.wikipedia.org/wiki/%E4%B8%AD%E7%BB%A7%E5%99%A8)
指將輸入訊號增強放大的類比裝置，而不考慮輸入訊號種類（類比或是數位）。
中繼器是用來加強纜線上的訊號，把訊號送得更遠，以延展網路長度。
當電子訊號在電纜上傳送時，訊號強度會隨著傳遞長度的增加而遞減。
因此需要中繼器將訊號重新加強以增加資料的傳送距離。\
(https://zh.wikipedia.org/wiki/%E4%B8%AD%E7%BB%A7%E5%99%A8)
## [集線器(HUB)](https://zh.wikipedia.org/wiki/%E9%9B%86%E7%B7%9A%E5%99%A8)
指將多條乙太網路雙絞線或光纖集合連接在同一段物理媒介下的裝置。
集線器是運作在OSI模型中的實體層[1]，可以讓其連結的裝置工作在同一網段。\
(https://zh.wikipedia.org/wiki/%E9%9B%86%E7%B7%9A%E5%99%A8)
## [L7-Switch](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E4%BA%A4%E6%8F%9B%E5%99%A8#%E4%B8%83%E5%B1%82)
更加智慧型的交換器，可以充分利用頻寬資源來過濾，辨識和處理應用層資料轉換的交換裝置。
## [L4-Switch](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E4%BA%A4%E6%8F%9B%E5%99%A8#%E5%9B%9B%E5%B1%82)
四層交換器可以處理第四層傳輸層協定，可以將對談與一個具體的IP位址繫結，以實現虛擬IP。
## [L3-Switch](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E4%BA%A4%E6%8F%9B%E5%99%A8#%E4%B8%89%E5%B1%82)
三層交換器則可以處理第三層網路層協定，用於連接不同網段，通過對預設閘道器的查詢學習來建立兩個網段之間的直接連接。
三層交換器可以實現路由器的全部或部分功能，但只能用於同一類型的區域網路子網路之間的互連。這樣，三層交換器可以像二層交換器那樣通過MAC位址標識封包，也可以像傳統路由器那樣在兩個區域網
路子網路之間進行功能較弱的路由轉發，它的路由轉發不是通過軟體來維護的路由表，而是通過專用的ASIC晶片處理這些轉發。
## [L2-Switch](https://zh.wikipedia.org/wiki/%E7%B6%B2%E8%B7%AF%E4%BA%A4%E6%8F%9B%E5%99%A8#%E4%BA%8C%E5%B1%82)
二層交換器依據硬體位址（MAC 位址）在資料鏈路層（第二層）傳送網路影格。 二層交換器對於路由器和主機是「透明的」，主要遵從802.1d 標準。該標準規定交換器通過觀察每個埠的資料框獲得源
MAC 位址，交換器在內部的高速緩衝記憶體中建立MAC 位址與埠的對映表。當交換器接受的資料框的目的位址在該對映表中被查到，交換器便將該資料框送往對應的埠。如果它查不到，便將該資料框廣播
到該埠所屬虛擬區域網路（VLAN）的所有埠，如果有回應封包，交換器便將在對映表中增加新的對應關係。當交換器初次加入網路中時，由於對映表是空的，所以，所有的資料框將發往虛擬區域網路內的
全部埠直到交換器「學習」到各個MAC 位址為止。這樣看來，交換器剛剛啟動時與傳統的共享式集線器作用相似的，直到對映表建立起來後，才能真正發揮它的效能。這種方式改變了共享式乙太網路搶行
的方式，如同在不同的行駛方向上鋪架了立交橋，去往不同方向的車可以同時通行，因此大大提高了流量。從VLAN的角度來看，由於只有子網路內部的節點競爭頻寬，所以效能得到提高。主機1 存取主機
2 同時，主機3 可以存取主機4 。當各個部門具有自己獨立的伺服器時，這一優勢更加明顯。但是這種環境正發生巨大的變化，因為伺服器趨向於集中管理，另外，這一模式也不適合Internet的應用。不
同VLAN之間的通訊需要通過路由器來完成，另外為了實現不同的網段之間通訊也需要路由器進行互連。

``資料來源``
