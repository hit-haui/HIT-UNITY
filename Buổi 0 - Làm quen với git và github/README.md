# HIT-UNITY
## Buổi 0: Git, GitHub và những câu lệnh của Git cơ bản
### (1) Git
#### Khái niệm

<details><summary>Xem nội dung</summary>
- Có thể hiểu đơn giản. Git giống như một chiếc xe vận chuyển code để lưu trữ giữa máy tính (local) và kho github (remote).
  - Lưu trữ `mốc thời gian` code của bạn, điều này giúp bạn có thể trở về quá khứ để lấy lại code cũ do những sai sót trong lúc code
  - Tạo một `bản miêu tả` sơ qua những gì bạn muốn một cách vừa đẹp vừa dễ dàng với README.md
  - Các thao tác giúp bạn và mọi người `cùng làm dự án` một cách quy củ, hợp lí (phần này gồm rất nhiều chi tiết như branch, pull requests, ...)
  - .... Còn cả một kho tàng của GitHub nữa mà các bạn có thể đọc thêm ở [link này](https://en.wikipedia.org/wiki/GitHub)
- Git là một công cụ vận chuyển code bằng các câu lệnh máy tính thông qua một số phần mềm như GitBash, GitDesktop, ....
</details>

##### Các câu lệnh của git

<details><summary>Xem nội dung</summary>
- Làm quen với cách vận chuyển của GitBash thông qua một số câu lệnh thường dùng
  - `git status` ( Kiểm tra các file bị thay đổi đã được git quản lí hay chưa )
    * Xanh là được quản lí, đỏ là chưa được quản lí
  - `git add` ( Cấp quyền quản lí cho git quản lí )
    * git add "Tenfile" => thêm một file cho git quản lí
    * git add . , git add * => thêm tất cả file cho git quản lí
  - `git commit` ( Xác nhận và đánh dấu thời điểm git quản lí giữ liệu )
    * git commit -m "Message" => Tạo tiêu đề cho 
  - `git push` ( Đưa giữ liệu lên trên GitHub )
    * git push => Sẽ tự tìm đến đúng nhánh đang dùng để tải lên nhánh đó trên GitHub
    * git push + origin(remote) + "tên nhánh" => tải lên nhánh đó
  - `git clone` ( Tải về máy repos )
    * git clone + "Đường dẫn đến repos" => Chỉ để tải repos
  - `git pull` ( Cập nhật những cái trên repos trên mạng có mà repos trên máy ko có )
    * git pull => Tự tìm đến nhánh trên máy để pull về
</details>

- Cách tạo một file txt trên GitHub: vào phần `create new file` ở repos để tạo
  - Hình ảnh hướng dẫn [Xem thêm](image-guide-1.md)
- Cách thêm một người cho repos của bạn
  - Hình ảnh hướng dẫn [Xem thêm](image-guide-2.md)
  
### (2) Github
#### Khái niệm
- Github đơn giản là một cái mạng xã hội code, hay là một kho lưu trữ
  - Ở đây bạn hoàn toàn có thể lưu lại từng phần code của mình một. Cụ thể như sau
     - VD: Bạn có lưu code của project A. Sau đó bạn lại chỉnh sửa và code thêm vào. Bạn để git quản lí. Toàn bộ cấu trúc trong thư mục của mỗi lần bạn thêm, sửa, xóa sẽ được lưu bởi git.
  - Github cũng giống như một mạng xã hội. Hoàn toàn có thể chia sẻ code, viết những ý kiến vào trong project, ...
### (3) Tổng kết
- Giới thiệu và làm quen các thành viên trong lớp
- Biết tổng quan về Git, GitHub và các câu lệnh của Git
- Sử dụng các câu lệnh để có thể lưu trữ

