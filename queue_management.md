# Queue management
Queue la một kỹ thuật làm cơ sở cho mọi truyền thông các task và đồng bộ trong môi trường freeRTOS. Chúng là một chủ đề quan trọng không thể tránh được khi xây dựng những ứng dụng phức tạp với các task co-operating với task khác. Chúng được hiểu là để lưu trữ và độ dài dữ liệu có hạn (tên là "length"). 

Chúng cho phép đọc và ghi bởi vài task khác nhau, và không theo một task một cách riêng biệt. Một queue thường là một FIFO nghĩa là các thành phần được đọc trong khi đã được ghi. Cách xử lý này phụ thuộc vào phương thức ghi: hai function ghi có thể được sử dung để ghi hoặc tại lúc bắt đầu hoặc lúc kết thúc queue đó.
## Việc đọc trong một queue
Khi một task đơn đọc trong một queue, nó được chuyển tới trạng thái "Blocked" và đưa trở lại "Ready" ngay khi dữ liệu được ghi vào trong queue bởi một task khác hoặc một ngắt. Nếu có một số task cố gắng đọc một queue, task nào có mức ưu tiên cao nhất đọc đầu tiên. Cuối cùng, nếu có vài task có độ ưu tiên như nhau cố gắng đọc task, task yêu cầu đầu tiên được chọn. Một task cũng có thể được chỉ định một thời gian chờ tối đa để queue cho phép nó được đọc. Sau thời gian đó, task tự động chuyển lại trạng thái "Ready"

