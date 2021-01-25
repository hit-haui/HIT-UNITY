# Bài tập buổi 2

<details><summary>Yêu cầu cơ bản</summary>
 <p>Áp dụng bài tập ở Buổi 1</p>
 <p>Di chuyển nhân vật với Rigidbody2D.velocity. Không sử dụng Transform.position như bài trước</p>
 <p>Tạo một scene như hình bên dưới đây<p>
 <h5>Có thể hình khác nhưng các GameObject yêu cầu phải có</h5>
 <li>Rigidbody2D</li>
 <li>Collider2D (BoxCollider2D, CircleCollider2D,...)</li>
 <img src="https://user-images.githubusercontent.com/50346687/105737153-2e1fb700-5f68-11eb-8df0-5559638400f1.png"/>
 <p>Yêu cầu của bài di chuyển này là phải in ra Rigidbody.velocity ra ngoài màn hình Console. 
  <br/> Sử dụng Debug.Log(value) -> value in ra giá trị của biến cho vào. "Sơn" -> Console: string-Sơn. (int)32 -> Console: int-32
 <img src="https://user-images.githubusercontent.com/50346687/105737164-311aa780-5f68-11eb-9da4-545d8b11a550.png"/>
<p>Tiếp theo sử dụng </p>
<li>OnCollisionEnter2D</li>
<li>OnCollisionStay2D</li>
<li>OnCollisionExit2D</li>
<p>Debug.Log ra màn hình như hình dưới</p>
<img src="https://user-images.githubusercontent.com/50346687/105738898-1ba67d00-5f6a-11eb-9f9d-1d8ce5482f5c.png"/>
<h5>Làm thêm với Trigger</h5>
</details>
<details><summary>Yêu cầu nâng cao</summary>
 <li>Di chuyển với velocity. Bao gồm cả nhảy</li>
 <li>Xác định việc có đang đứng trên địa hình (ground) hay không</li>
 <h3>Gợi ý</h3>
 <li>Di chuyển thì nên sử dụng vector để mô tả lại lực di chuyển (Chú ý đến trọng lực)</li>
 <li>Sử dụng OnCollisionStay2D để xem có đang va chạm với địa hình (ground)</li>
</details>
