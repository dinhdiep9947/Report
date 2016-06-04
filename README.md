# Hệ thống Real Time là gì?
_______________________________
Một hệ thống thời gian thực được thiết kế cho các nhiệm vụ đặc biêt:
  * Các ứng dụng cần được thực thi với thời gian thật chính xác, các lỗi phát sinh cần được cô lập và xử lý nhanh chóng.
  * Phải đáp lại các ngõ vào hay các sự kiện với thời gian giới hạn.
  * Một đáp ứng trễ là một đáp ứng sai.

# freeRTOS là gì?
________________________________
freeRTOS là một hệ thế thống Real-Time miễn phí và mã nguồn mở được phát triển bởi Real Time Engineers Ltd. Mục đích của nó phát triển vừa cho các hệ thống nhúng rất nhỏ và chỉ bổ sung các chức năng rất tối thiểu:
  * Cho phép nhiều chương trình thực thi tại cùng một thời điểm (multi-tasking).
  * Sử dụng các tác vụ rất cơ bản và quản lý bộ nhớ.
  * API chỉ đủ cho việc đồng bộ hóa.


![](RTOS.png)

Quy luật của hệ thống freeRTOS:
* Thời gian yêu cầu cho việc hoàn thành bất kỳ các function nào phải có hạn và có thể biết trước.
* Thời gian phản hồi tối đa phải tính toán được và được đảm bảo.
* Số chu kỳ yêu cầu để thực thi một toán tử đã cho phải luôn như nhau.
* Việc thực thi có bị ngắt nhưng độ trễ ngắt và thời gian xử lý phải được ngăn chặn.

Những đối tượng không cần RTOS:
* Các ứng dụng với một mục đích.
* Các ứng dụng vòng lặp đơn giản và polling.
* Các ứng dụng tiêu biểu nhỏ hơn 32kBytes.

Chúng ta không cần RTOS để viết phần mềm nhúng hiệu quả nhưng ứng dụng dần dần tăng kích thước và độ phức tạp thì RTOS sẽ rất hữu ích.





