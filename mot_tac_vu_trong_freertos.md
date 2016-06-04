# Một tác vụ trong FreeRTOS
FreeRTOS không giới hạn số lượng các tác vụ có thể chạy miễn sao phần cứng và bộ nhớ có thể điều khiển được. FreeRTOS cho phép điều khiển cả các tác vụ có chu kỳ và không có chu kỳ.

## Vòng đời của một tác vụ
Phần này sẽ mô tả chính xác hơn nữa về cách có thể gọi ra một tác vụ từ lúc nó được tạo ra cho tới khi nó bị hủy. Ở đây, chúng ta sẽ xem chỉ có sẵn duy nhất một nhân vi xử lý, nghĩa là chỉ một sự tính toán hay chỉ một tác vụ có thể chạy tại thời điểm đã cho. Bất kỳ tác vụ đã cho có một trong hai trạng thái: "running" và "not running". Như chúng ta đã giả định rằng chỉ có một lõi, một tác vụ có thể chạy tại một thời điểm đã cho; mọi tác vụ khác trong trạng thái "not running". Khi một tác vụ chuyển trạng thái từ "not running" sang "running", ta gọi đó là "swapped in" hay "switched in", ngược lại là "swapped out" hay "switched out".

*CMSIS RTOS đưa ra task như Thread, trong bài này task được dùng thay thế nghĩa cho thread*





