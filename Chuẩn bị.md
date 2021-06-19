### Những thứ cần chuẩn bị trước khi cài đặt Hackintosh

​	Việc cài đặt một hệ điều hành máy tính thường khá đơn giản và không tốn quá nhiều thời gian. Tất cả mọi người đều có thể cài đặt một phiên bản Window, Linux, FreeBSD v.v. một cách dễ dàng (có lẽ không cần viết một bài hướng dẫn 😄) trên gần như mọi hệ thống máy tính. Nhưng không giống như cài đặt các hệ điều hành khác, MacOS là một hệ điều hành được Apple sinh ra chỉ có thể cài đặt duy nhất trên những thiết bị do Apple sản xuất và kiểm soát khắt khe. Vậy nên việc "qua mặt" hệ thống MacOS, đánh lừa nó rằng nó đang được cài đặt trên một thiết bị của Apple là một việc rất khó khăn, phức tạp. Tuy nhiên khi hoàn thành hệ thống Hackintosh hoàn toàn có thể vận hành mượt mà và ổn định như máy real Mac.

​	**Vậy nên, thứ đầu tiên cần phải chuẩn bị đó là tâm lý, thời gian và sự kiên nhẫn. **

​	Nếu bạn cần gấp, hoặc có công việc quan trọng, hoặc đơn giản chỉ muốn một máy tính chạy MacOS để làm việc thì hãy bỏ tiền ra mua một chiếc MacOS đi, hoặc nếu tài chính không cho phép thì có thể thuê thợ cài Hackintosh (như các bạn ra quán nhờ cài win vậy) với phí khoảng trên 400k (tham khảo từ một người bạn, mình cũng k rõ giá thị trường, còn dao động tùy vào cấu hình nữa), tất nhiên là bạn phải có sẵn một thiết bị có phần cứng phù hợp (sẽ được nói ở phần chuẩn bị phần cứng).

​	Bạn nên bắt đầu hành trình này với tinh thần học hỏi, thử thách bản thân, trải nghiệm. Mục đích sử dụng chỉ nên đứng thứ 2 thôi. Bạn có thể sẽ mất cả tuần (thậm chí hơn nữa) để hệ thống của bạn có thể sử dụng một cách bình thường, để đầy đủ tính năng và hoạt động ổn định thì còn lâu hơn nữa. Tuy nhiên khi đã hoàn thành việc này, nó sẽ là một trải nghiệm đáng giá, xứng đáng với công sức và thời gian bạn bỏ ra.

​	Khi bắt đầu, bạn nên chuẩn bị tâm lý rằng Hackintoshes không phải là thứ mà bạn nên dựa vào như một cỗ máy làm việc. Nó vẫn sẽ hữu ích trong công việc nhưng chỉ sau khi hoàn thành, và có khả năng bạn sẽ không hoàn thành được nó nên đừng quá trông đợi khi bắt đầu. Ngoài ra, nên nhớ rằng MacOS k phù hợp để chơi game, tùy theo nhu cầu các bạn có thể cài đặt song song MacOS và Window.

​	Sau khi hoàn thành hành trình gian nan này, chúng ta sẽ có những lợi ích sau:

- Trải nghiệm hệ điều hành MacOS mượt mà, những tính năng thú vị (iCloud, iMessage, Facetime, Airdrop v.v.) cùng với khả năng đồng bộ với các thiết bị khác trong hệ sinh thái của Apple.
- Cấu hình cao, hiệu năng trên giá thành cực tốt so với máy real Mac.
- Có thể sử dụng các phần mềm độc quyền của MacOS (Cá nhân mình biết đến Hackintosh vì cần sử dụng Xcode). 
- Thiết kế đa dạng, kiến thức mới v.v.

​	Từ những điều trên và nhu cầu của bản thân, hãy quyết định có nên bắt tay vào Hackintosh hay không.

​	**Điều thứ hai cần chuẩn bị là kiến thức.**

​	Bạn cần phải biết cài đặt các hệ điều hành khác, hiểu biết về cách hệ điều hành hoạt động (đặc biệt là Unix và các Unix-like), các phần cứng, ví dụ như:

- Tên Cpu của bạn và thế hệ của nó
- Tên GPU( aka VGA aka Card đồ họa)
- Ổ cứng
- Chipset ethernet
- Chipset WLAN/Bluetooth

> Cách xác định cụ thể sẽ được nói ở phần sau

​	Một thứ quan trọng nữa là các bạn cần phải hiểu biết cơ bản về command lines, cách sử dụng terminal/command prompt. Nếu bạn là một người dùng Linux thì mọi thứ sẽ trở nên dễ dàng hơn đôi chút. Các bạn có thể tìm hiểu ít nhất là cách truy cập thư mục, copy hoặc xóa tệp bằng command lines. Còn nếu bạn không biết gì về máy tính thì bài này để đọc cho vui thôi.

​	**Cuối cùng là phần cứng và các thiết bị liên quan.**

​	Tối thiểu các bạn cần một hệ thống máy tính, một USB để tạo bộ cài MacOS. Tuy nhiên sẽ rất khó khăn và rủi ro cao vì cài Hackintosh rất dễ gây hỏng hệ điều hành đang chạy. Vậy nên tốt nhất là nên có 2 hệ thống máy tính - một để tạo bộ cài, cấu hình bộ cài và search google :v và một để cài đặt. Sau đây là chi tiết về các phần cứng tương thích (khả dụng để cài đặt Hackintosh).

- **USB**: tối thiểu 8GB, khuyên dùng 16GB. Cái này không quá khó khăn nên tốt nhất nên chuẩn bị một USB 16GB tránh trường hợp giữa chừng phát hiện ra thiếu dung lượng thì vừa mất công vừa khó chịu.
- **Ổ cứng**: theo cá nhân mình, có một lưu ý quan trọng đối với vấn đề lưu trữ nên cần đưa lên trước những linh kiện như CPU, GPU v.v. Cụ thể:
  - Nên sử dụng SSD, ít nhất là 120GB để cài đặt hệ điều hành vì tốc độ truy xuất của nó, sau đó lắp thêm HDD dung lượng lớn để lưu trữ dữ liệu hoặc dùng luôn ổ cứng SSD dung lượng lớn nếu có điều kiện. Tất nhiên việc sử dụng hoàn toàn HDD cũng khả dụng, tuy nhiên sẽ mang lại trải nhiệm khá tệ (chạy một hệ điều hành mượt mà trên một thiết bị chậm như rùa :v).
  - **Có một số mẫu SSD cần lưu ý**, đó là:
    -  SSD Samsung PM981, PM991, Micron 2200S và những ổ cứng Intel 600p là những mẫu không nên (rất rất rất không nên) cài Hackintosh. Nếu cài đặt trên những ổ cứng này sẽ gây ra lỗi Kernel panic - một lỗi của hệ điều hành Unix và các Unix-like - tương tự như lỗi màn hình xanh ở window, có một điểm khác biệt đáng chú ý là hệ thống sẽ không thể tự khắc phục và vượt qua, buộc người dùng phải tìm cách sửa lỗi hoặc cài lại hệ điều hành nếu lỗi quá nghiêm trọng. Có thể sử dụng NVMeFix.kext để cài đặt thành công nhưng sẽ không thể khắc phục triệt để vấn đề và vẫn có thể gây ra một số sự cố khởi động (boot issues).
    -  SSD WDC Green (các mẫu WD khác như Blue hay Red không có nguồn thông tin nào nhắc đến, nhưng tốt nhất nên tránh nếu muốn mua ổ cứng mới, nếu đang sử dụng các mẫu này thì có thể thử :v) không hỗ trợ định dạng APFS mới hơn của Apple, bắt buộc dùng HFS. Tức là bạn vẫn có thể cài đặt Hackintosh nhưng cần lưu ý về định dạng ổ cứng.
    -  SSD Samsung 970 EVO PLUS cần phải update firmware mới nhất (Download firmware từ website của samsung, Sử dụng công cụ balenaEtcher để tiến hành update. Khá đơn giản và chỉ mất vài phút, chi tiết hơn các bạn có thể search google). 
  - Laptop sử dụng công nghệ Intel Optane không được hỗ trợ trên MacOS (không rõ đối với desktop). Bạn vẫn có thể cài đặt phiên bản MacOS 10.15 (Catalina) trên những thiết bị này nhưng sẽ tiềm ẩn những rủi ro về vấn đề khởi động (boot).
  - Việc cài đặt Hackintosh sẽ không làm hỏng ổ cứng của bạn, tuy nhiên nếu quá trình chuẩn bị thiếu chu đáo dẫn đến format, ghi xóa dữ liệu quá nhiều lần sẽ ảnh hưởng xấu đến tuổi thọ ổ cứng. Hãy chuẩn bị mọi thứ thật cẩn thận và không cần lo lắng cho ổ cứng của bạn.
- **CPU**: Phần lớn các CPU đều có thể (chỉ là có thể thôi nhé) cài đặt Hackintosh. Tuy nhiên cần lưu ý:
  - CPU của AMD chỉ hỗ trợ 3 thế hệ Bulldozer(15th), Jaguar(16th) và Ryzen(17th) (có lẽ 2 thế hệ trước không nhiều người biết, chỉ phổ biến Ryzen) và những CPU cho laptop **không được hỗ trợ**. Ngoài ra, một số tính năng của MacOS sẽ **không khả dụng** trên CPU AMD desktop. Hiện tại mình không có CPU ADM desktop nên k thể thử nghiệm thực tế trường hợp này.
  - Phần lớn các CPU Intel **cho Desktop** đều hỗ trợ Hackintosh, dòng Pentium, Atom và Celeron sẽ cần phải fakecpuid thành Core i.  
  - CPU Intel **cho Laptop** chỉ hỗ trợ dòng  Core i và Xeon
  - Bạn cũng phải lưu ý về iGPU, cụ thể: dòng Xeon k có iGPU, các dòng Pentium, Atom  và Celeron mặc dù có iGPU nhưng không được hỗ trợ, iGPU của dòng Core i từ trước thế hệ thứ 3 không được hỗ trợ, những trường hợp này cần phải có GPU rời. 
- **GPU:** MacOS khá kén linh kiện này. Những điều cần chú ý là:
     - AMD: Đa số các AMD đều có thể cài đặt Hackintosh, ngoại trừ:
          - Các AMD APU - các chip tích hợp cả CPU và GPU tương tự như các chip tích hợp iGPU của Intel. Tất cả các dòng chip này đều k thể cài đặt Hackintosh.
          - Các GPU Lexa dựa trên kiến trúc Polaris (phổ biến nhất là các dòng RX 500 series) không được hỗ trợ. Điều này chưa rõ ràng, đây là một lưu ý khi sử dụng OpenCore bootloader nhưng những thợ cài chuyên nghiệp cho rằng dòng RX500 series hoàn toàn có thể chạy tốt Hackintosh. Có lẽ những bạn sử dụng dòng GPU này nên chọn Clover bootloader để cài đặt. 
          - Riêng GPU MSI Navi RX 5700 XT không thể cài đặt Hackintosh do một lỗi xảy ra trong GPUInfo framework, đã có người khắc phục được nhưng khá phức tạp và không tổng quát. Lỗi này không xuất hiện ở MacOS 11 (Big Sur) nhưng đây là phiên bản MacOS mới nhất nên sẽ chưa có  sự hỗ trợ đầy đủ từ cộng đồng nên mình không khuyên dùng. Tất nhiên các bạn vẫn có thể thử nhưng sẽ khá vất vả. [Đây](https://github.com/acidanthera/bugtracker/issues/901) là đường dẫn nói về lỗi này và cách khắc phục nếu các bạn muốn tìm hiểu.
     - Nvidia: Các dòng GPU của Nvidia có rất nhiều điều cần lưu ý:
          - Kiến trúc Kepler (600 & 700 series) sẽ được hỗ trợ đầy đủ nhất, trên mọi phiên bản MacOS.
          - Kiến trúc Maxwell (900 series) và Pascal (1000 series) chỉ hỗ trợ những phiên bản MacOS 10.13 (High Sierra) trở về trước.
          - Các kiến trúc mới hơn như Turing (2000 series) và Ampere (3000 series) sẽ không hỗ trợ bất cứ phiên bản MacOS nào (Do Apple đã không còn hợp tác với Nvidia từ năm 2019).
     - iGPU: Chip GPU tích hợp của Intel. Như đã nói ở phần CPU, chỉ duy nhất iGPU của các CPU dòng Core i từ thế hệ thứ 3 trở về sau có thể hoạt động trên MacOS, đồng nghĩa với việc những CPU Intel còn lại sẽ phải đi kèm với GPU rời để hoạt động.
     - **Một lưu ý quan trọng** đối với các GPU rời **trên Laptop**: 90% GPU rời sẽ không hoạt động, các bạn sẽ phải ngắt kết nối và tắt nó đi. Một số trường hợp dùng được  cũng sẽ không ổn định, thường xuyên gặp vấn đề. Mình sẽ cài đặt trên một máy laptop chạy GTX 1050 để hướng dẫn chi tiết phần này.
- **Mainboard/Motherboard**: Tất cả các mainboard đều có thể cài đặt Hackintosh (với CPU thích hợp), lưu ý rằng MacOS không thể xuất hình ảnh qua cổng VGA (hỗ trợ DVI, HDMI và Displayport) nên nếu main của bạn chỉ có công VGA (chắc là rất hiếm loại này) thì sẽ cần GPU rời hoặc ... một chiếc main khác.
- **Kết nối mạng**: một trong những vấn đề đau đầu của những Hackintosh-er. 
     - Sẽ là đơn giản nếu thiết bị của bạn có thể kết nối mạng bằng dây. Phần lớn các wired network adapter **đều được hỗ trợ** bởi các drivers có sẵn của MacOS hoặc kexts do cộng đồng người dùng tạo ra. Có một số thiết bị khó khăn trong việc cấu hình nhưng cũng có những giải pháp khắc phục triệt để. 
     - **Hầu hết các Wifi card trên laptop sẽ không được hỗ trợ chính thức** từ MacOS (ngoại trừ card Atheros của Qualcomm có thể chạy phiên bản MacOS 10.13 trở về trước và các mẫu card của Broadcom, những mẫu này trên laptop thường k nhiều). Những chiếc laptop sử dụng card Wifi của Intel phổ biến hơn lại không được hỗ trợ, tuy nhiên có một số kext do cộng đồng phát triển có thể giúp những thiết bị này hoạt động được, mình sẽ thử nghiệm ở quá trình cài đặt. Bạn cũng có thể sử dụng các thiết bị Adapter Wifi dạng USB, nhưng những thiết bị này sẽ gây lỗi ảnh hưởng đến việc sleep/wakeup máy. **Tất cả những vấn đề này sẽ được hướng dẫn chi tiết ở phần cấu hình, cài đặt.**
- **Ram:** Không có thông tin cụ thể về các thông số như DDR, bus. Có lẽ chúng ta chỉ cần quan tâm đến dung lượng RAM, tương tự như các hệ thống máy tính ở thời điểm hiện tại, mình khuyên dùng mức RAM 8GB trở lên, tối thiểu có lẽ 4GB là chạy được.
- **Những thành phần khác:**
     - Cảm biến vân tay: không thể cài đặt.
     - Camera: Những thiết bị có camera kết nối bằng chuẩn USB có thể hoạt động được (nếu bạn may mắn :v ), còn những thiết bị có camera kết nối bằng I2C sẽ không hoạt động được. Mình không có đủ dữ kiện để xác minh thông tin này, trong quá trình cài đặt sẽ thử nghiệm trên máy của mình.
     - Micro của Laptop và các vấn đề khác của jack cắm tai nghe, mình sẽ thử nghiệm khi cài đặt.
     - Cổng Thunderbolt USB-C gặp một số lỗi, đơn giản nhất là disable Thunderbolt và sử dụng như một cổng USB-C thông thường, vẫn có những cách khác để sử dụng Thunderbolt, mình sẽ thử nghiệm khi cài đặt.

### Tổng quát lại toàn bộ quy trình chuẩn bị

​	**Tinh thần**: tự chuẩn bị

​	**Backup dữ liệu:** Một bước cơ bản khi cài đặt bất cứ hệ điều hành nào, toàn bộ dữ liệu trong phân vùng cài đặt hệ điều hành sẽ bị mất. 

​	**Xác định phần cứng**: Xác định phần cứng sẵn có và so sánh với những lưu ý phía trên, đảm bảo mọi thứ tương thích và mua thêm những linh kiện còn thiếu.

​	**Công cụ:** USB tối thiểu 8GB, khuyên dùng 16GB trở lên, Internet (download bộ cài khá nặng, và các tool, kext cần thiết), nên có một máy tính thứ 2 để hỗ trợ quá trình cài đặt.

​	

