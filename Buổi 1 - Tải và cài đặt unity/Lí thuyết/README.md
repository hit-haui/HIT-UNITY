# Lý Thuyết

## TÌM HIỂU VỀ UNITY ENGINE

<details><summary>CLICK TO SEE</summary>
###	Các thành phần trong Unity Editor
<body >
<p><img src="https://images.viblo.asia/a8b99650-c3fd-43f2-939b-fc8f0fa8fa19.png" alt="" data-src="https://images.viblo.asia/a8b99650-c3fd-43f2-939b-fc8f0fa8fa19.png" data-zoom-src="https://images.viblo.asia/full/a8b99650-c3fd-43f2-939b-fc8f0fa8fa19.png" srcset="https://images.viblo.asia/retina/a8b99650-c3fd-43f2-939b-fc8f0fa8fa19.png 2x"></p>
<h3>1.Cửa sổ Sences</h3>
<ul>
<li>Phần này phần hiển thị các đối tượng trong scenes một cách trực quan, có thể lựa chọn các đối tượng, kéo thả, phóng to, thu nhỏ, xoay các đối tượng ...</li>
<li>Phần này có để thiết lập một số thông số như hiển thị ánh sáng, âm anh, cách nhìn 2D hay 3D ...
-Khung nhìn Scene là nơi bố trí các Game Object như cây cối, cảnh quan, enemy, player, camera, … trong game. Sự bố trí hoạt cảnh là một trong những chức năng quan trọng nhất của Unity.</li>
</ul>
<h3>2.Cửa sổ Hierarchy</h3>
<ul>
<li>Tab hierarchy là nơi hiển thị các Game Object trong Sences hiện hành. Khi các đối tượng được thêm hoặc xóa trong Sences, tương ứng với các đối tượng đó trong cửa sổ Hierarchy.</li>
<li>Tương tự trong tab Project, Hierarchy cũng có một thanh tìm kiếm giúp quản lý và thao tác với các Game Object hiệu quả hơn đặc biệt là với các dự án lớn.</li>
</ul>
<h3>3.	Cửa sổ Game</h3>
<ul>
<li>Đây là mạn hình demo Game, là góc nhìn từ camera trong game.</li>
<li>Thanh công cụ trong cửa sổ game cung cấp các tùy chỉnh về độ phân giải man hình,        thông số (stats), gizmos, tùy chọn bật tắt các component...</li>
</ul>
<h3>4.	Cửa sổ Project</h3>
<ul>
<li>Đây là cưa sổ explorer của Unity, hiển thị thông tin của tất cả các tài nguyên (Assets) trong game của bạn.</li>
<li>Cột bên trái hiển thị assets và các mục yêu thích dưới dạng cây thư mục tương tự như Windows Explorer. Khi click vào một nhánh trên cây thư mục thì toàn bộ nội dung của nhánh đó sẽ được hiển thị ở khung bên phải. Ta có thể tạo ra các thư mục mới bằng cách Right click -&gt; Create -&gt; Folder hoặc nhấn vào nút Create ở góc trên bên trái cửa sổ Project và chọn Folder. Các tài nguyên trong game cũng có thể được tạo ra bằng cách này.</li>
<li>Phía trên cây thư mục là mục Favorites, giúp chúng ta truy cập nhanh vào những tài nguyên thường sử dụng. Chúng ta có thể đưa các tài nguyên vào Favorites bằng thao tác kéo thả.</li>
<li>Đường dẫn của thư mục tài nguyên hiện tại. Chúng ta có thể dễ dàng tiếp cận các thư mục con hoặc thư mục gốc bằng cách click chuột vào mũi tên hoặc tên thư mục.</li>
</ul>
<h3>5.	Cửa sổ Inspector</h3>
<ul>
<li>Cửa sổ Inspector hiển thị chi tiết các thông tin về Game Object đang làm việc, kể cả những component được đính kèm và thuộc tính của nó. Bạn có thể điều chỉnh, thiết lập mọi thông số và chức năng của Game Object thông qua cửa sổ Inspector.</li>
<li>Mọi thuộc tính thể hiện trong Inspector đều có thể dễ dàng tuỳ chỉnh trực tiếp mà không cần thông qua một kịch bản định trước. Tuy nhiên Scripting API cung cấp một số lượng nhiều và đầy đủ hơn do giao diện Inspector là có giới hạn.</li>
<li>Các thiết lập của từng component được đặt trong menu. Các bạn có thể click chuột phải, hoặc chọn icon hình bánh răng nhỏ để xuất hiện menu.</li>
<li>Ngoài ra Inspector cũng thể hiện mọi thông số Import Setting của asset đang làm việc như hiển thị mã nguồn của Script, các thông số animation, …</li>
</ul>
<h2>II.	 Các khái niệm cơ bản trong unity</h2>
<h3>1.	GameObject</h3>
<p>Một đối tượng cụ thể trong game gọi là một game object, có thể là nhân vật, đồ vật nào đó.
Ví dụ: cây cối, xe cộ, nhà cửa, người...</p>
<h3>2.	Component</h3>
<p>Một GameObject sẽ có nhiều thành phần cấu tạo nên nó như là hình ảnh (sprite render), tập hợp các hành động (animator), thành phần xử lý va chạm (collision), tính toán vật lý (physical), mã điều khiển (script), các thành phần khác... mỗi thứ như vậy gọi là một component của GameObject.</p>
<h3>3. Sprite</h3>
<p>Là một hình ảnh 2D của một game object có thể là hình ảnh đầy đủ, hoặc có thể là một bộ phận nào đó.</p>
<h3>4. Animation</h3>
<p>Là tập một hình ảnh động dựa trên sự thay đổi liên tục của nhiều sprite khác nhau.</p>
<h3>5. Key Frame</h3>
<p>Key Frame hay Frame là một trạng thái của một animation. Có thể được tạo nên từ 1 sprite hay nhiều sprite khác nhau.</p>
<h3>6. Prefabs</h3>
<p>Là một khái niệm trong Unity, dùng để sử dụng lại các đối tượng giống nhau có trong game mà chỉ cần khởi tạo lại các giá trị vị trí, tỉ lệ biến dạng và góc quay từ môt đối tượng ban đầu.
Ví dụ: Các đối tượng là đồng tiên trong game Mario đều có xử lý giống nhau, nên ta chỉ việc tạo ra một đối tượng ban đầu, các đồng tiền còn lại sẽ sử dụng prefabs. Hoặc khi ta lát gạch cho một cái nền nhà, các viên gạch cũng được sử dụng là prefabs.</p>
<h3>7. Sounds</h3>
<p>Âm thanh trong game.</p>
<h3>8. Script</h3>
<p>Script là tập tin chứa các đoạn mã nguồn, dùng để khởi tạo và xử lý các đối tượng trong game.
Trong Unity có thể dùng C#, Java Script, BOO để lập trình Script.</p>
<h3>9. Scenes</h3>
<p>Quản lý tất cả các đối tượng trong một màn chơi của game.</p>
<h3>10. Assets</h3>
<p>Bao gồm tất cả những gì phục vụ cho dự án game như sprite, animation, sound, script, scenes…</p>
<h3>11. Camera</h3>
<p>Là một game object đặc biệt trong scene, dùng để xác định tầm nhìn, quansát các đối tượng khác trong game.</p>
<h3>12. Transform</h3>
<p>Là 3 phép biến đổi tịnh tiến, quay theo các trục, và phóng to thu nhỏ một đối tượng</p>
</details>

 
