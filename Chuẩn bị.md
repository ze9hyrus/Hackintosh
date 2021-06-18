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
    -  SSD Samsung PM981, PM991 và Micron 2200S không thể cài Hackintosh (Nếu cài đặt sẽ gây ra lỗi Kernel panic - một lỗi của hệ điều hành Unix và các Unix-like - tương tự như lỗi màn hình xanh ở window, có một điểm khác biệt đáng chú ý là hệ thống sẽ không thể tự khắc phục và vượt qua, buộc người dùng phải tìm cách sửa lỗi hoặc cài lại hệ điều hành nếu lỗi quá nghiêm trọng) . 
    - SSD WDC Green (các mẫu WD khác như Blue hay Red không có nguồn thông tin nào nhắc đến, nhưng tốt nhất nên tránh nếu muốn mua ổ cứng mới, nếu đang sử dụng các mẫu này thì có thể thử :v) không hỗ trợ định dạng APFS mới hơn của Apple, bắt buộc dùng HFS. Tức là bạn vẫn có thể cài đặt Hackintosh nhưng cần lưu ý về định dạng ổ cứng.
    - SSD Samsung 970 EVO PLUS cần phải update firmware mới nhất (Download firmware từ website của samsung, Sử dụng công cụ balenaEtcher để tiến hành update. Khá đơn giản và chỉ mất vài phút, chi tiết hơn các bạn có thể search google).
- **CPU**: Phần lớn các CPU đều có thể (chỉ là có thể thôi nhé) cài đặt Hackintosh. Tuy nhiên cần lưu ý:
  - CPU của AMD chỉ hỗ trợ 3 thế hệ Bulldozer(15th), Jaguar(16th) và Ryzen(17th) (có lẽ 2 thế hệ trước không nhiều người biết, chỉ phổ biến Ryzen) và những CPU cho laptop **không được hỗ trợ**. Ngoài ra, một số tính năng của MacOS sẽ **không khả dụng** trên CPU AMD. Hiện tại mình không có CPU ADM desktop nên k thể thử nghiệm thực tế trường hợp này.
  - Phần lớn các CPU Intel **cho Desktop** đều hỗ trợ Hackintosh, dòng Pentium, Atom và Celeron sẽ cần phải fakecpuid thành Core i.  
  - CPU Intel **cho Laptop** chỉ hỗ trợ dòng  Core i và Xeon
  - Bạn cũng phải lưu ý về iGPU, cụ thể: dòng Xeon k có iGPU, các dòng Pentium, Atom  và Celeron mặc dù có iGPU nhưng không được hỗ trợ, iGPU của dòng Core i từ trước thế hệ thứ 3 không được hỗ trợ, những trường hợp này cần phải có GPU rời. 
- **GPU:** 

