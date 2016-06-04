# Chức năng cơ bản của một RTOS
1. Bộ lập lịch (Scheduler)
2. Các dịch vụ thời gian thực (Realtime Services)
3. Đồng bộ và xử lý thông điệp (Synchronization và Messaging)

## Scheduler
Mỗi tác vụ có thể có 1 trong ba trạng thái chính:
* **Ready to rung:** là trạng thái mà tác vụ đã đủ các tài nguyên để khởi chạy nhưng chưa chạy. Đây là trạng thái chuẩn bị của tác vụ.
* **Running:** là trạng thái mà tác vụ đang được thực thi.
* **Blocked:** khi tác vụ không có đủ các tài nguyên cần thiết để chạy thì nó sẽ được đưa về trạng thái này.

Để lập lịch cho tác vụ, có 3 kỹ thuật được áp dung:
* **Co-operative scheduling:** mỗi task được thực thi đến khi kết thúc quá trình thì task tiếp theo mới được thực thi.



