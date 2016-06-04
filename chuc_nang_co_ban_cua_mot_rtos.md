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
* **Co-operative scheduling** 
  * Giống như code thông thường.
  * Các task chỉ có thể được thực thi nếu task đang chạy "give up"/yield.
* **Round Robin Scheduling:** mỗi task được chia một khe thời gian cố định, nếu trong khoảng thời gian được chia đó mà task chưa thực hiện xong thì sẽ bị tạm dừng, chờ đến lượt tiếp theo để thực hiện tiếp công việc sau khi hệ thống xử lý hết một lượt các task.



