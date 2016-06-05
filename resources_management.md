# Resources management
## Binary semaphores
Binary semaphores là cách đơn giản hiệu quả nhất để đồng bộ các task, một cách cũng đơn giản hơn nữa, nhưng không mang lại hiệu quả, phù hợp trong polling một input hay 1 resource. Một binary semaphore có thể xem như một queue mà nó chỉ gồm có 1 element.
![](Untitled11.png)
## Mutexes
Mutexes được thiết kế để ngăn chặn việc loại trừ lẫn nhau hay việc đình trệ. Một mutex được sử dụng tương tự như một binary semaphore, trừ việc task lấy semaphore đó phải gửi lại. Điều nàu có thể thông qua với một token đã liên kết với resource để truy cập vào. Một task giữ token, làm việc với resource sau đó trả lại token. Trong lúc đó, không có một token nào khác được đưa cho mutex.


