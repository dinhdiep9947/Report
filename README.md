# FreeRTOS

FreeRTOS là một hệ thống Real-Time Operating miễn phí và mã nguồn mở được phát triển bởi Real Time Engineers Ltd. Mục đích là để phát triển vừa với những hệ thống nhúng rất nhỏ và  chỉ bổ sung những hàm rất tối thiểu: điều khiển rất cơ bản của các tác vụ (task) và quản lý bộ nhớ, chỉ đủ API về việc đồng bộ hóa, và hoàn toàn không cung cấp truyền thông internet, các driver cho mở rộng phần cứng, hay truy cập vào một filesystem. Tuy nhiên, chúng có đặc điểm sau:
- Các tác vụ có chiếm quyền ưu tiên trước.
- Hỗ trợ 23 kiến trúc vi xử lý bởi các nhà phát triển.
- Footprint nhỏ (4.3Kbytes trên ARM7 sau khi biên dịch).
- Viết bằng C và biên dịch với nhiều trình biên soạn C.
Nó cũng cho phép số lượng tác vụ không giới hạn chạy cùng một thời gian và  không giới hạn mức ưu tiên của chúng miễn là phần cứng có thể đáp ứng được. Cuối cùng, nó bổ sung hàng đợi (queues), binary và counting semaphores và mutexes.