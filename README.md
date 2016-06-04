# Hệ thống RTOS là gì?
_______________________________
Một hệ thống thời gian thực (RTOS - Real Time Operating System) được thiết kế cho các nhiệm vụ đặc biêt:
  * Các ứng dụng cần được thực thi với thời gian thật chính xác, các lỗi phát sinh cần được cô lập và xử lý nhanh chóng.
  * Phải đáp lại các ngõ vào hay các sự kiện với thời gian giới hạn.
  * Một đáp ứng trễ là một đáp ứng sai.


![](RTOS.png)

Quy luật của hệ thống RTOS:
* Thời gian yêu cầu cho việc hoàn thành bất kỳ các function nào phải có hạn và có thể biết trước.
* Thời gian phản hồi tối đa phải tính toán được và được đảm bảo.
* Số chu kỳ yêu cầu để thực thi một toán tử đã cho phải luôn như nhau.
* Việc thực thi có bị ngắt nhưng độ trễ ngắt và thời gian xử lý phải được ngăn chặn.

Những đối tượng không cần RTOS:
* Các ứng dụng với một mục đích.
* Các ứng dụng vòng lặp đơn giản và polling.
* Các ứng dụng tiêu biểu nhỏ hơn 32kBytes.

Chúng ta không cần RTOS để viết phần mềm nhúng hiệu quả nhưng ứng dụng dần dần tăng kích thước và độ phức tạp thì RTOS sẽ rất hữu ích.





