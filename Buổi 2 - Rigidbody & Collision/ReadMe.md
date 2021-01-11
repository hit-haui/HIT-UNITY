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
  <li>Dynamic: Như tên gọi, loại này cho phép cả nội lực (bao gồm các lực mà từ vật này sinh ra, velocity, thường thì sử dụng code) và ngoại lực (bao gồm trọng lực) tác động vào GameOject </li><p>
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
  <h5>Một phần khá thú vị là hệ thống Joint của Unity. Các bạn sẽ tìm hiểu cái này sau khi hiểu về Rigidbody và Collision. Đừng tham, tẩu hỏa nhập ma đấy!</h5>
  </details> 
</details>
<details><summary>Collision2D</summary>
  <p>Collision là va chạm </br>Collider là vật va chạm</br> Vậy, hệ thống này sử dụng để mô phỏng va chạm giữa các vật thể với nhau (các GameOject đều yêu cầu có Collider 2D)
  <p>Có các loại Collider 2D khác nhau: Box Collider 2D, Casule Collider 2D, Circle Collider 2D,... Tùy thuộc vào hình dạng của sprite để sử dụng cho hợp lý. Tất cả đều có các thuộc tính giống nhau nên ở đây sẽ tìm hiểu về BoxCollider2D</p>
  <img src="https://user-images.githubusercontent.com/50346687/104216725-04956480-546d-11eb-8153-8b1e16cb3b26.png"/>
  <details><summary>Vùng va chạm (khu vực mà có thể va chạm với các vật thể khác)</summary>
  <li>Size: size của Vùng va chạm :))</li>
  <li>Offset: Vị trí bị lệch trên hệ tọa độ Oxy so với gốc ban đầu của Vùng va chạm </li>
  <li>Edit Collider: Điều chỉnh được Vùng va chạm trực tiếp trên Scene Window. </li>
  </details>
  <details><summary>Một số thuộc tính quan trọng khác</summary>
  <li>IsTrigger: Vẫn là vùng va chạm, nhưng chỉ nhận thông tin của Vật tác động vào Vùng va chạm này chứ không tác động lên vật.</li>
  <li>Used By Composite: Vùng va chạm sẽ liền thành một khối. Sử dụng cho TileMap chúng ta học trong những buổi tiếp theo.</li>
  <li>Material: Tương tự như Material của Rigidbody</li>
  </details>
  <p>Ngoài ra, Collider rất cần thiết cho hệ thống RayCast sau này</p>
</details>
