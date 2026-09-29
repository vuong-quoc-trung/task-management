# BỐI CẢNH

Chúng tôi là một công ty phần mềm quy mô vừa. Hiện tại công ty có nhiều đội phát triển cùng lúc nhiều dự án.

Hiện nay các nhóm đang quản lý công việc bằng nhiều công cụ khác nhau như bảng tính, tin nhắn và tài liệu riêng. Điều này khiến việc theo dõi tiến độ, phân công công việc và kiểm tra lịch sử thay đổi trở nên khó khăn.

Chúng tôi muốn xây dựng một hệ thống quản lý công việc nội bộ để các nhóm có thể quản lý dự án và công việc tập trung trên một nền tảng.

Hệ thống cần đủ linh hoạt để một công ty có thể có nhiều dự án, một dự án có nhiều thành viên và mỗi thành viên có thể tham gia nhiều dự án khác nhau.

---

# MỤC TIÊU

Hệ thống cần giúp công ty:

* Quản lý người dùng và thành viên trong các dự án.
* Tạo và quản lý các dự án.
* Chia công việc thành các task.
* Phân công task cho thành viên.
* Theo dõi trạng thái và tiến độ công việc.
* Cho phép các thành viên trao đổi về task.
* Theo dõi lịch sử hoạt động của dự án.
* Hỗ trợ người quản lý theo dõi tiến độ của nhóm.

---

# NGƯỜI SỬ DỤNG

Hệ thống có nhiều loại người dùng với các trách nhiệm khác nhau.

### Người quản trị hệ thống

Có trách nhiệm quản lý người dùng và các vấn đề liên quan đến toàn bộ hệ thống.

### Người quản lý dự án

Có trách nhiệm quản lý các dự án mà họ phụ trách, thành viên trong dự án và công việc của dự án.

### Thành viên dự án

Có thể tham gia các dự án được phân công và thực hiện các công việc của mình.

Hiện tại chúng tôi chưa xác định chi tiết tất cả quyền hạn của từng loại người dùng. Chúng tôi muốn nhóm phát triển phân tích và đề xuất cách tổ chức quyền phù hợp.

---

# CÁC YÊU CẦU NGHIỆP VỤ BAN ĐẦU

## Người dùng

Người dùng cần có tài khoản để sử dụng hệ thống.

Người dùng có thể đăng nhập vào hệ thống.

Thông tin của người dùng có thể được quản lý và cập nhật.

---

## Dự án

Người có quyền phù hợp có thể tạo một dự án mới.

Mỗi dự án có một số thông tin cơ bản như tên, mô tả và thông tin liên quan đến tiến độ.

Một dự án có thể có nhiều thành viên.

Một người dùng có thể tham gia nhiều dự án.

Khi dự án không còn hoạt động, nó có thể được đóng lại.

---

## Thành viên dự án

Người quản lý cần có khả năng thêm người dùng vào dự án.

Thành viên có thể được loại khỏi dự án.

Các thành viên trong cùng một dự án có thể có trách nhiệm hoặc quyền hạn khác nhau.

---

## Task

Người có quyền phù hợp có thể tạo task trong một dự án.

Mỗi task cần có thông tin để mô tả công việc.

Task có thể được giao cho một thành viên.

Task có trạng thái để thể hiện tình hình xử lý.

Task có thể có mức độ ưu tiên.

Task có thể có thời hạn.

Task có thể được cập nhật trong quá trình thực hiện.

---

## Bình luận

Thành viên dự án có thể trao đổi về một task thông qua bình luận.

Một task có thể có nhiều bình luận.

Bình luận cần gắn với người tạo và thời điểm tạo.

---

## Theo dõi hoạt động

Hệ thống cần cho phép người dùng xem các hoạt động quan trọng đã xảy ra trong dự án hoặc task.

Ví dụ:

* Một task được tạo.
* Task được giao cho một người.
* Trạng thái task thay đổi.
* Thành viên được thêm vào dự án.
* Có người đăng bình luận.

Chúng tôi muốn có lịch sử để biết những thay đổi quan trọng đã xảy ra.

---

## Tiến độ

Người quản lý cần có khả năng theo dõi tình hình của dự án.

Hệ thống nên cung cấp thông tin giúp người quản lý biết:

* Có bao nhiêu task.
* Có bao nhiêu task đã hoàn thành.
* Có bao nhiêu task đang thực hiện.
* Có bao nhiêu task chưa bắt đầu.
* Có những task nào gần hoặc đã quá hạn.

---

# MỘT SỐ YÊU CẦU CHUNG

Hệ thống sẽ được sử dụng bởi nhiều người trong cùng thời điểm.

Dữ liệu của các dự án phải được phân tách hợp lý. Người dùng không được xem hoặc thay đổi dữ liệu của những dự án mà họ không có quyền truy cập.

Hệ thống cần lưu lại những thay đổi quan trọng để có thể kiểm tra khi cần.

Chúng tôi muốn giao diện dễ sử dụng và có thể sử dụng trên máy tính.

---

# PHẠM VI BAN ĐẦU

Ở phiên bản đầu tiên, chúng tôi muốn tập trung vào:

```text
User
Project
Project Member
Task
Comment
Task Status
Task Priority
Activity History
```

Chúng tôi chưa quyết định có cần các chức năng như:

```text
File attachment
Email notification
Real-time notification
Recurring task
Subtask
Task dependency
Time tracking
Calendar
Report nâng cao
Mobile application
```

Các chức năng này có thể được xem xét sau.

---

# MỘT SỐ VẤN ĐỀ CHÚNG TÔI CHƯA XÁC ĐỊNH

Chúng tôi chưa có câu trả lời cuối cùng cho một số vấn đề như:

* Một task có thể được giao cho nhiều người hay chỉ một người?
* Ai được tạo project?
* Ai được xóa project?
* Thành viên có tự rời project được không?
* Ai được thay đổi trạng thái task?
* Ai được sửa hoặc xóa comment?
* Task quá hạn được xử lý như thế nào?
* Project đóng rồi có được sửa task không?
* Người dùng thuộc nhiều project thì quyền của họ có giống nhau ở mọi project không?
* Có cần giữ lịch sử của mọi thay đổi hay chỉ những thay đổi quan trọng?
* Có cần xóa dữ liệu thật sự hay chỉ đánh dấu là không còn hoạt động?

Chúng tôi mong nhóm phát triển đặt câu hỏi để làm rõ những điểm này trước khi bắt đầu xây dựng hệ thống.

---

# KẾT QUẢ MONG MUỐN

Chúng tôi muốn có một hệ thống mà nhân viên có thể sử dụng hàng ngày để:

```text
Đăng nhập
   ↓
Xem dự án
   ↓
Xem thành viên
   ↓
Xem task
   ↓
Nhận task
   ↓
Cập nhật task
   ↓
Bình luận
   ↓
Theo dõi tiến độ
```

Và người quản lý có thể:

```text
Tạo project
   ↓
Thêm thành viên
   ↓
Tạo / phân công task
   ↓
Theo dõi tiến độ
   ↓
Kiểm tra lịch sử hoạt động
```

Đây là toàn bộ thông tin chúng tôi có thể cung cấp ở giai đoạn đầu.

Nhóm phát triển cần chủ động đặt câu hỏi và phân tích yêu cầu trước khi đưa ra giải pháp kỹ thuật.
