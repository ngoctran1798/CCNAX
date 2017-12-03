Người Thực Hiện: Trần Thị Ngọc  
Ngày Cập Nhật: 07/11/2017   
-----   
## 1.Entheret là gì?    
![imgur](https://i.dowload.vn/data/image/2017/07/10/LAN-Ethernet-10.jpg)  
**Ethernet là một trong số những phương tiện mà bạn có thể sử dụng để tạo ra một mạng LAN, bao gồm cả Wi-Fi, Bluetooth và USB.Những thứ này có thể được sử dụng để tạo ra một mạng cục bộ hoặc có thể cùng tồn tại trong cùng một mạng.** Trong khi mạng không dây có sự tiện lợi riêng của nó thì Ethernet vẫn giữ nhiều vai trò quan trọng, như:

  - Ethernet vẫn là kết nối facto cho những máy trạm trong các mạng doanh nghiệp.  
  - Kể cả khi trong mạng không dây hoàn chỉnh (mạng gia đình) thì kết nối giữa cáp / DSL modem và router là Ethernet.  
  - Các hoạt động băng thông như chơi trò chơi hay phát trực tuyến vẫn được hưởng lợi từ kết nối Ethernet có dây.  
  - Mạng Ethernet tiếp tục cung cấp lợi ích của bảo mật vật lý.  
  
*Ethernet là 1 công nghệ mạng cục bộ (LAN) nhằm chuyển thông tin giữa các máy tính với tốc độ từ 10 đến 100 triệu bít một giây (Mbps) . Hiện thời công nghệ Ethernet thường được sử dụng nhất là công nghệ sử dụng cáp đôi xoắn 10-Mbps. Công nghệ truyền thông 10-Mbps sử dụng hệ thống cáp đồng trục cỡ lớn , hoặc cáp đôi , cáp sợi quang . Tốc độ chuẩn cho hệ thống Ethernet hiện nay là 100-Mbps .*  

- Ethernet chuẩn thường có cấu hình bus, truyền với tốc độ 10Mbps và dựa vào CSMA/CD (Carrier SenseMultipleAccess / CollisionDetection) để điều chỉnh lưu thông trên đường cáp chính.
- Cấu hình: bus hoặc star.
- Phương pháp chia sẻ môi trường truyền: CSMA/CD.
- Cáp: cáp đồng trục gầy, cáp đồng trục béo, cáp UTP.
- Tên của chuẩn Ethernet thể hiện 3 đặc điểm sau:
- Con số đầu tiên thể hiện tốc độ truyền tối đa.
- Từ tiếp theo thể hiện tín hiệu dải tần cơ sở được sử dụng (Base hoặc Broad). Các ký tự còn lại thể hiện loại cáp được sử dụng.
![Imgur](https://i.imgur.com/SKEknv3.jpg)


## 2.Tìm hiểu cấu trúc Ethernet Frame?

![Imgur](https://i.imgur.com/x4aSC0X.png)

**Cấu trúc gồm:**

- **Preamble (8 bytes)**: được sử dụng cho các hoạt động đồng bộ frame trong cách thức truyền dữ liệu của Ethernet
- **Dest Address (6 bytes)**: cho biết địa chỉ MAC của thiết bị mà thiết bị này gửi đến.
Source Address (6 bytes): cho biết địa chỉ MAC của thiết bị gửi frame.
- **Type/Length (2 bytes)**: cho biết chiều dài của phần data, cung cấp giá trị dùng để xác định phần data đang chứ dữ liệu của giao thức nào Vd: Type là 0x0806 data này đang đóng gói một gói tin ARP.
- **Data:** dữ liệu được truyền tải bởi Ethernet frame.
- **FCS (4 bytes):** được dùng để check lỗi của frame Ethernet.

-----
## 3.LAN Standards?
**Mạng LAN (mạng nội bộ) là một hệ thống truyền thông cho phép kết nối và chia sẻ các tài nguyên giữa các thiết bị độc lập trong một khu vực địa lý có kích thước vừa phải. Các chủ đề này giới thiệu các loại mạng cục bộ được hỗ trợ bởi hệ thống iSeries ™:**

- **Mạng DDI (giao diện dữ liệu phân tán)**
	- FDDI là một mạng cục bộ dựa trên cáp quang (LAN) sử dụng tiêu chuẩn 3T9.5 của Tiêu chuẩn Quốc gia Hoa Kỳ (ANSI) cho một giao thức kiểm soát truy cập truyền thông qua thẻ tín hiệu. Các trạm, bộ khuếch đại, và cầu trong một mạng FDDI được kết nối vật lý với một trong những vòng quay quay ngược hoặc cả hai vòng quay quay ngược. Các vòng hoạt động ở tốc độ 100 Mbps.
	- Mạng FDDI cho phép các thiết bị được gắn vào một hoặc cả hai vòng. Thông thường chỉ có vòng sơ cấp trong mạng FDDI đang hoạt động. Vòng đệm thứ cấp được sử dụng để duy trì mạng khi trạm truy cập kép hoặc bộ tập trung không hoạt động.
- **Ethernet:**
	*Ethernet là một kiểu topo mạng cục bộ (LAN) được hỗ trợ bởi hệ điều hành. i5 / OS ™ Ethernet cung cấp hỗ trợ cho Tổng công ty Thiết bị kỹ thuật số, Tổng công ty Intel, và chuẩn Xerox (Ethernet Version 2) và tiêu chuẩn IEEE 802.3.*
	- Half-duplex Ethernet
		- Nói chung, nhiều trạm trong một mạng Ethernet cho thấy một con đường dữ liệu duy nhất. Do đó, chỉ một trạm có thể truyền dữ liệu tại một thời điểm. Đây được gọi là half-duplex Ethernet. Trạm chỉ có thể truyền hoặc nhận, nhưng không đồng thời.
	- Ethernet toàn song song
		- Ethernet Full-duplex cho phép các trạm đồng thời gửi và nhận dữ liệu trên mạng, loại bỏ va chạm. Điều này được thực hiện thông qua việc sử dụng một switch LAN full-duplex. Chuyển mạch Ethernet chia tách một Ethernet lớn thành các phân đoạn nhỏ hơn. Full-duplex Ethernet đòi hỏi những điều sau đây:
			- Truyền dẫn cáp xoắn đôi vừa
			- Thẻ giao diện mạng Ethernet
			- Một switch LAN full-duplex
		- Hỗ trợ 10 Mbps Ethernet đồng thời có kết nối 10 Mbps và 10 Mbps gửi đi.
	- Fast Ethernet
		-Tiêu chuẩn Fast Ethernet (IEEE 802.3U) tăng Ethernet bằng tốc độ hoạt động từ 10 Mbps đến 100, half hoặc full duplex.
		- Bộ điều hợp Ethernet iSeries ™ hỗ trợ các thiết bị mạng 100BASE-TX sử dụng cáp xoắn kép được che chắn và không được che chở (STP, UTP).
- **Mạng Token-ring:**
	*Mạng token-ring là một cấu trúc liên kết LAN gửi dữ liệu theo một hướng trong suốt một số vị trí cụ thể bằng cách sử dụng mã thông báo. Mã thông báo là biểu tượng của quyền kiểm soát đường truyền. Mã thông báo này cho phép bất kỳ trạm phát nào trong mạng (vòng) gửi dữ liệu khi mã thông báo đến nơi đó.*
	*Các trạm trong mạng token-ring được kết nối vật lý, điển hình là trong topo vòng có dây sao, tới bộ tập trung dây, chẳng hạn như Bộ phận truy cập đa luồng đa năng của IBM 8228. Bộ tập trung hoạt động như một vòng hợp lý xung quanh dữ liệu được truyền ở tốc độ 4 triệu, 16 triệu hoặc 100 triệu bit mỗi giây (Mbps). Mỗi trạm được nối với máy tập trung thông thường bằng cáp xoắn kép được bảo vệ (STP).*
	- Vòng mã thẻ hai mặt
		- Trong vòng token full-duplex, còn được gọi là DTR (vòng mã thông báo dành riêng), các nút chuyển mạch cho phép các trạm gửi và nhận dữ liệu trên mạng đồng thời. Một hub chuyển mạch token-ring chia mạng thành các phân đoạn nhỏ hơn. Khi một trạm phát gói dữ liệu của nó, chuyển đổi vòng token đọc thông tin địa chỉ đích của gói tin và chuyển tiếp dữ liệu trực tiếp đến trạm nhận. Công tắc sau đó thiết lập một kết nối chuyên dụng giữa hai trạm, cho phép dữ liệu được truyền và nhận cùng một lúc. Trong vòng mã thông báo full-duplex, giao thức token-passing bị treo. Mạng có hiệu lực trở thành một vòng tròn tokenless 'tokenless'. Vòng mã thông báo full-duplex tăng khả năng gửi và nhận băng thông cho các trạm kết nối, nâng cao hiệu năng mạng.
		
-----
## 4.Địa chỉ MAC? Cấu trúc địa chỉ MAC.
- Địa chỉ phần cứng được sử dụng trong Ethernet LAN (hardware address hay physical address) được biết đến với tên gọi địa chỉ MAC. MAC address gồm 48 bit nhị nhân thường biểu diễn dưới dạng hexa, địa chỉ này là duy nhất cho từng thiết bị, không trùng với bất cứ thiết bị nào trên thới giới.
- Cấu trúc của một địa chỉ MAC:

![Imgur](https://i.imgur.com/oeE2QOM.jpg)

Trong đó:

- OUI – Organizationally Unique Identifier: 3 byte ở phần đầu địa chỉ MAC dùng để định danh cho các nhà sản xuất thiết bị.
- Vendor Assigned: 3 byte do nhà sản xuất định danh cho thiết bị.

---
## 5.Broadcast Domain và Collisions Domaim?
- Collision domain:
	- Là các segment mạng vật lý được kết nối ở đó có các đụng độ có thể xảy ra.
	- Mỗi khi một đụng độ xảy ra trên mạng, tất cả các hoạt động truyền dừng lại trong một khoảng thời gian.
	- Thiết bị thuộc lớp 1 không chia tách miền đụng độ mà chỉ mở rộng miền đụng độ.
	- Thiết bị thuộc lớp 2 và 3 chia tách miền đụng độ thành các miền đụng độ nhỏ hơn (sự phân đoạn mạng – segmentation).
- Broadcast domain:
	- Một broadcast domain là một nhóm các miền đụng độ được kết nối bởi các thiết bị lớp 2.
	- Các gói tin broadcast nếu nhiều quá mức có thể làm giảm hiệu suất của mạng LAN.
	- Broadcast được kiểm soát bởi thiết bị lớp 3. Router có thể phân chia các broadcast domain.
- Cách xác định :
	- Một Port của Router là 1 Broadcast Domain
	- Các port Router được nối lại với nhau chỉ tính là 1
	- Một port của SW, router là một Collision Domain
	- Các port của SW, Router nối lại với nhau chỉ tính là 1
	- Hub là 1 Collision Domain

----
## 6.So sánh việc truyền tải giữa Hub và Switch?
![Imgur](https://i.imgur.com/0Ql6Ihi.jpg)

*Hub và switch cả hai thiết bị này đều có những vai trò tương tự trên mạng. Mỗi thiết bị dều đóng vai trò kết nối trung tâm cho tất cả các thiết bị mạng, và xử lý một dạng dữ liệu được gọi là “frame” (khung). Mỗi khung đều mang theo dữ liệu. Khi khung được tiếp nhận, nó sẽ được khuyếch đại và truyền tới cổng của PC đích. Sự khác biệt lớn nhất giữa hai thiết bị này là phương pháp phân phối các khung dữ liệu.*

- Điểm giống nhau của HUB và SWITCH:
	- Cả hai thiết bị đều làm nhiệm vụ mở thêm Port nhằm kết nối nhiều máy tính lại với nhau.
	- Cả hai đều có chức năng khuếch đại tín hiệu ngỏ vào.
- Điểm khác nhau giữa HUB và SWITCH.
	- HUB có 3 loại là
		+ Passive Hub: (Hub thụ động)
		+ Active Hub: (Hub chủ động)
		+ Intelligent Hub: (Hub thông minh)
		+ Ngoại trừ HUB thông minh làm việc ở tầng 2 trong mô hình OSI giống với SWITCH thì HUB chỉ làm việc ở tầng 1 tương tự như thiết bị Repeater. Ngoài ra thiết bị Passive HUB không dùng đến nguồn điện phụ nên nó hoạt động rất kém và số port rất thấp.

		+ Với hub, một khung dữ liệu được truyền đi hoặc được phát tới tất cả các cổng của thiết bị mà không phân biệt các cổng với nhau. Việc chuyển khung dữ liệu tới tất cả các cổng của hub để chắc rằng dữ liệu sẽ được chuyển tới đích cần đến. Tuy nhiên, khả năng này lại tiêu tốn rất nhiều lưu lượng mạng và có thể khiến cho mạng bị chậm đi (đối với các mạng công suất kém).Ngoài ra, một hub 10/100Mbps phải chia sẻ băng thông với tất cả các cổng của nó. Do vậy khi chỉ có một PC phát đi dữ liệu (broadcast) thì hub vẫn sử dụng băng thông tối đa của mình. Tuy nhiên, nếu nhiều PC cùng phát đi dữ liệu, thì vẫn một lượng băng thông này được sử dụng, và sẽ phải chia nhỏ ra khiến hiệu suất giảm đi.

	- Ở Switch có một bộ nhớ được biết như là buffer làm nhiệm vụ lưu trử thông tin các Host mà nó quản lý bao gồm IP và Physical Address, cơ chế này giúp cho Switch thực hiện đựơc tính năng chuyển mạch. Switch chủ yếu làm việc trên tầng 2 OSI, một số Switch chuyên dụng làm việc trên tầng 3 OSI, hay còn gọi là Switch Layer 3.-+ Điểm khác nhau quan trọng trong qúa trình chuyển Frame của HUB và SWITCH. Trong khi HUB luôn luôn chuyển frame theo dạng Broadcast (gữi thông tin đi toàn bộ các Note trong mạng) thì ngược lại Switch chỉ gữi Broadcart ở lần đầu tiên để cập nhật thông tin vào bộ nhớ còn từ đó về sau nó luôn chuyển thông tin theo kiểu end to end chứ không gữi Broadcast nữa. Switch layer 3 có thêm phần định tuyến tương tự như Router và chức năng V-LAN (mạng LAN ảo) còn HUB hoàn toàn ko có chức năng này.

	- Switch lưu lại bản ghi nhớ địa chỉ MAC của tất cả các thiết bị mà nó kết nối tới. Với thông tin này, switch có thể xác định hệ thống nào đang chờ ở cổng nào. Khi nhận được khung dữ liệu, switch sẽ biết đích xác cổng nào cần gửi tới, giúp tăng tối đa thời gian phản ứng của mạng. Và không giống như hub, một switch 10/100Mbps sẽ phân phối đầy đủ tỉ lệ 10/100Mbps cho mỗi cổng thiết bị. Do vậy với switch, không quan tâm số lượng PC phát dữ liệu là bao nhiêu, người dùng vẫn luôn nhận được băng thông tối đa. Đó là lý do tại sao switch được coi là lựa chọn tốt hơn so với hub.

----
## 7.Phương pháp CSMA/CD?
**Carrier Sense Multiple Access with Collision Detect (viết tắt CSMA/CD)** trong tiếng Anh, nghĩa là đa truy cập nhận biết sóng mang phát hiện xung đột. Đây là một trong nhiều phương pháp truy cập hay sử dụng trong mạng LAN, cải tiến từ phương pháp CSMA. Theo phương pháp này, khi một máy tính muốn truyền một gói tin, trước tiên nó sẽ lắng nghe xem trên đường truyền có sóng mạng hay không (bằng cách lắng nghe tín hiệu Carrier). Nếu không có, nó sẽ thực hiện truyền gói tin (theo frame). Sau khi truyền gói tin, nó vẫn tiếp tục lắng nghe để xem có máy nào định truyền tin hay không. Nếu không có xung đột, máy tính sẽ truyền gói tin cho đến hết. Nếu phát hiện xung đột, nó sẽ gửi broadcast một gói tin báo hiệu cho các máy trên mạng không nên gửi tin để tránh làm nhiễu đường truyền,sau đó chờ một khoảng thời gian ngẫu nhiên trước khi tiến hành gửi lại gói tin. Tiến trình các bước như sau: 

- Một thiết bị có frame cần truyền sẽ lắng nghe đường truyền cho đến khi nào đường truyền Ethernet không còn bị chiếm.
- Khi đường truyền Ethernet không còn bị chiếm, máy gửi bắt đầu gửi frame.
- Máy gửi cũng bắt đầu lắng nghe để đảm bảo rằng không có xung đột xảy ra.
- Nếu có xung đột, tất cả các máy trạm đã từng gửi ra frame sẽ gửi ra một tín hiệu nghẽn để đảm bảo tất cả các máy trạm đều nhận ra xung đột.
- Sau khi tín hiệu nghẽn là hoàn tất, mỗi máy gửi của những frame bị xung đột sẽ khởi động một bộ định thờI (timer) và chờ hết khoản thời gian này sẽ cố gắng truyền lại. Những máy không tạo ra xung đột sẽ không phải chờ.
- Sau khi các thời gian định thời là hết, máy gửi có thể bắt đầu một lần nữa với bước 1.

*CSMA/CD được phát triển từ CSMA để tăng hiệu quả của phương thức CSMA, bằng cách dừng việc truyền tín hiệu ngay khi phát hiện thấy xung đột, giảm thiểu thời gian chờ để thực hiện việc truyền tiếp theo. (CSMA không kết thúc việc truyền dữ liệu nếu phát hiện xung đột, những máy đang truyền sẽ tiếp tục truyền, những máy gây xung đột sau khi nhận được thông báo sẽ dừng một khoảng thời gian trước khi cố gắng truyền tiếp).*

-----
## 8.ARP? Cơ chế hoạt động của ARP trong cùng LAN? Khác LAN?
Trong hệ thống mạng máy tính có hai loại địa chỉ được gán cho một máy tính:

- Địa chỉ logic: là địa chỉ của các giao thức mạng như IP, IPX … Loại địa chỉ này mang tính chất tương đối, có thể thay đổi theo sự cần thiết của người sử dụng. Loại địa chỉ này có hai phần: Phần network để phân định hoạt động của máy trong các mạng khác nhau và giúp dễ dàng định tuyến cho các gói tin cần chuyển đi giữa các interface của các router,  phần Host để phân biệt các máy trong cùng một mạng.
- Địa chỉ vật lý – MAC (Media Access Control) là địa chỉ tuyệt đối, ghi chết vào thiết bị giao tiếp, trong thực tế các NIC (Network Interface Card) chỉ có thể hiểu và liên lạc với nhau bằng địa chỉ này.

Vì vậy, để các máy có thể liên lạc được với nhau trong môi trường mạng, cần phải có một cơ chế diễn giải địa chỉ giữa IP và MAC, đó là **giao thức Address Resolution Protocol viết tắt là  ARP.** 

**Hoạt động của một ARP trong mạng LAN:** 

Khi một thiết bị mạng muốn biết địa chỉ MAC của một thiết bị mạng nào đó một mạng LAN nó sẽ gửi một ARP request bao gồm địa chỉ MAC address của nó và địa chỉ IP của thiết bị mà nó cần biết MAC address trên toàn bộ một miền broadcast. Mỗi một thiết bị nhận được request này sẽ so sánh địa chỉ IP trong request với địa chỉ tầng network của mình. Nếu trùng địa chỉ thì thiết bị đó phải gửi ngược lại cho thiết bị gửi ARP request một gói tin (trong đó có chứa địa chỉ MAC của mình). Lúc này, A đã biết MAC id của máy tính cần gửi và như thế PC A mới bắt đầu truyền gói tin cho B. 

![Imgur](https://i.imgur.com/ItHrRhA.gif)

**Hoạt động của ARP trong môi trường liên mạng:**

Hoạt động của ARP trong một môi trường phức tạp hơn đó là hai (hay nhiều) hệ thống mạng gắn với nhau thông qua một Router 1. Máy A thuộc mạng A muốn gửi gói tin đến máy B thuộc mạng B. Do các broadcast không thể truyền qua Router nên khi đó máy A sẽ xem Router 1 như một cầu nối hay một trung gian (Agent) để truyền dữ liệu. Chúng ta cần hiểu rằng, trước đó máy A đã biết được địa chỉ IP của Router 1 thông qua khai báo Gateway trong các thông tin địa chỉ máy, khi trong IP của máy cần gửi đi không thuộc miền broatcast sẽ phải gửi gói tin qua 1. Tất cả các thông tin về các mạng sẽ được chứa trong một bảng gọi là bảng định tuyến (routing table), là thông tin về các Gateway để truy cập vào một hệ thống mạng nào đó và được lưu giữ trong mỗi máy. Ví dụ trong trường hợp trên trong bảng sẽ chỉ ra rằng để đi tới LAN B phải qua port X của Router 1. Như vậy khi truyền thông tin giữa các máy tính trong môi trường liên mạng, router đóng vai trò trung gian cung cấp thông tin.

*Quá trình truyền dữ liệu theo từng bước sau :*
 
- Máy A gửi một ARP request (broadcast) để tìm địa chỉ MAC của port X.
- Router ® trả lời, cung cấp cho máy A địa chỉ MAC của port X.
- Máy A truyền gói tin đến port X của Router trong đó có địa chỉ IP của máy B.
- Router nhận được gói tin từ máy A, chuyển gói tin ra port Y của Router. Dĩ nhiên trong gói tin có chứa địa chỉ IP của máy B. Router sẽ gửi ARP request để tìm địa chỉ MAC của máy B.
- Máy B sẽ trả lời cho Router biết địa chỉ MAC của mình. Sau khi nhận được địa chỉ MAC của máy B,Router 1 gửi gói tin của A đến B .


