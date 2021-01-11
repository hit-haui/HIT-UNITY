# Buổi 2: Rigidbody & Collision
## Yêu cầu thực hành. Nghịc các thông số của 2 Component này. 
## Lý thuyết
<details><summary>Rigidbody2D</summary>
  <p>Nguồn tham khảo đầu tiên => Unity Documentation</br>Các bạn đọc kết hợp giữa Unity docs và docs trên Github, nếu có không hiểu đoạn nào thì nhắn tin trong nhóm. Tập dần cho quen đi thôi!!!<p>
  [Unity Docs](https://docs.unity3d.com/Manual/class-Rigidbody2D.html)
  <h5>Rigidbody2D là gì? </h5><p>Rigidbody2D là hệ thống mô phỏng vật lý dành cho game2D (Không sử dụng cho 3D), ví dụ trọng lực, lực tác động, lực ma sát,... </p>
  <p>Bắt đầu tập trung vào những điểm sau</p>
  <img src ="https://user-images.githubusercontent.com/50346687/104209081-d8c1b100-5463-11eb-8003-6724afa4bb2f.png"/>
  <details><summary>Body Type</summary>
  <li>Dynamic: Như tên gọi, loại này cho phép cả nội lực (bao gồm các lực mà từ vật này sinh ra, thường thì sử dụng code) và ngoại lực (bao gồm trọng lực) tác động vào GameOject </li><p>
  <li>Kinematic: Loại này chỉ cho phép nội lực tác động vào GameOject</li>
  <li>Static: Không tác động lực vào được</li>
  <h4>Chú ý</h4><p>Có một chú ý ở đây, khi các bạn tìm hiểu kỹ hơn về Physics. Hệ thống Physics sẽ có Transform riêng, nó tự động cập nhật cho bằng Transform của GameOject sau mỗi FixedUpdate() được thực hiện. Với tất cả các loại ở đây sẽ tác động vào Transform của Rigidbody. Transform của GameObject tự động cập nhận theo Rigidbody. Nên nếu ta tác động vào Transform của GameObject thì Object vẫn di chuyển.
  </details>
  <details><summary>Material</summary>
  <p>Phần này sẽ liên quan đến Ma Sát và Độ nảy của GameObject</p>
  <p>Physics Materials 2D</p>
  <img src="https://user-images.githubusercontent.com/50346687/104211768-107e2800-5467-11eb-99a1-3c855ffc6aaa.png"/>
  <img src="https://user-images.githubusercontent.com/50346687/104212138-75398280-5467-11eb-94ec-97f7850c84f3.png"/>
  <li>Friction: Giá trị từ 0-1. 0 là không ma sát, 1 là độ ma sát max</li>
  <li>Bounciness: Giá trị từ 0-1. 0 là không nảy, 1 là max nảy</li>
  </details>
  <details><summary>Drag</summary>
  <li>Linear Drag: hệ số cản di chuyển, hệ số càng cao thì càng cần nhiều lực để di chuyển Rigidbody</li>
  <li>Angular Drag: hệ số cản quay, hệ số càng cao thì càng cần nhiều lực để quay Rigidbody</li>
  </details>
  <details><summary>Gravity</summary>
  <li>Mass: Nó là khối lượng đấy</li>
  <li>Gravity Scale: Mặc định là 9.81 (học trong vật lý rồi nhỉ :v) scale thì 1 là 9.81. 0 là 0 :)
  </details>
  <details><summary>Các thông số khác nâng cao hơn</summary>
  <li>Collision Detection: Khi vật đi xuyên qua dù đã có Collision thì tìm tài liệu ở đây</li>
  <li>Sleeping Mode: Thời gian Rigidbody hoạt động và nghỉ</li>
  <li>Interpolate: Phần này có ích khi di chuyển mượt mà hay cần ổn định</li>
  <li>Constraints: Khóa :)) thử đi sẽ biết</li>
  <h3>Trên [Unitydocs](https://docs.unity3d.com/Manual) có hết nhá. Khi tìm hiểu được những phần bên trên thì cũng nên tự tìm hiểu về các phần này</h3>
  </details> 
</details>
<details><summary>Rigidbody2D</summary>
</details>
