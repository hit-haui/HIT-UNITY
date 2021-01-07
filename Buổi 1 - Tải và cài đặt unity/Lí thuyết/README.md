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

### Các hàm chính trong thư viện Monobehaviour
<body class="post-template-default single single-post postid-610 single-format-standard wp-custom-logo">
<h4><span id="Mo_dau">Mở đầu</span></h4>



<ul><li>Trước tiên để tìm hiểu về các hàm được cung cấp sẵn, mình sẽ đưa ra sơ đồ tổng quát của <em>Unity3D Documentation</em> sau.</li><li>Mặc định trong bài viết các gameObjects được <span class="ph_keyword">active</span> cùng một lúc nhé</li></ul>



<div class="wp-block-image"><figure class="aligncenter"><img src="https://docs.unity3d.com/uploads/Main/monobehaviour_flowchart.svg" alt="monobehaviour_flowchart."><figcaption>Monobehaviour Flowchart (Unity3D Documents)</figcaption></figure></div>



<h2><span id="I_Initialization">I. Initialization</span></h2>



<p>Như chúng ta thấy ở bảng trên, <span class="ph_keyword">Awake</span>, <span class="ph_keyword">OnEnable</span> và <span class="ph_keyword">Start</span> nằm cùng một phần gọi là <span class="ph_keyword">Initialization</span> nhưng công dụng của chúng khác nhau như thế nào?, và chúng được gọi khi nào trong vòng đời của MonoBehaviour?</p>



<ul><li><strong>Awake<em>: </em></strong>các hàm <span class="ph_keyword">Awake</span> đều được gọi trước <strong>TẤT CẢ</strong> các hàm <span class="ph_keyword">Start</span> của các <em>MonoBehaviour </em>có trong Scene (được enable cùng lúc) hay gọi ngay sau khi gameObject đó được sinh ra bằng hàm <span class="ph_keyword">Instantiate()</span>.</li></ul>



<p><span class="ph_keyword">Awake</span> chỉ được gọi một lần duy nhất trong vòng đời của một <em>MonoBehaviour</em></p>



<ul><li><strong>OnEnable<em>:</em></strong> hàm này được gọi khi một gameObject được đổi trạng thái từ <em>deactive -&gt; active</em> hoặc khi enable <span class="ph_keyword">Component</span> và được gọi lần đầu tiên ngay sau hàm <span class="ph_keyword">Awake</span> của nó.</li></ul>



<p class="ph_question">“Vậy nếu có 2 gameObjects A và B thì thứ tự gọi có phải là Awake A -&gt; Awake B -&gt; OnEnable A -&gt; OnEnable B?”</p>



<p>Không, vào lúc active lần đầu tiên, thứ tự gọi như sau: </p>



<div class="wp-block-image"><figure class="aligncenter size-large"><img loading="lazy" width="677" height="186" src="https://phuongne.com/wp-content/uploads/2020/04/image.png" alt="awake-onenable" class="wp-image-684" srcset="https://phuongne.com/wp-content/uploads/2020/04/image.png 677w, https://phuongne.com/wp-content/uploads/2020/04/image-300x82.png 300w" sizes="(max-width: 677px) 100vw, 677px"><figcaption>Thứ tự gọi của Awake() và OnEnable() của 2 gameObjects bất kỳ</figcaption></figure></div>



<p class="ph_question">“Sao Awake của B gọi trước Awake của A vậy?”</p>



<p>Thứ tự gọi <span class="ph_keyword">Awake</span> trong Unity là random.</p>



<ul><li><strong>Start<em>:</em></strong> hàm <span class="ph_keyword">Start()</span> được gọi sau <span class="ph_keyword">OnEnable</span>, trước khi các frames bắt đầu chạy hay trước các hàm <span class="ph_keyword">Update</span>. Cũng như <span class="ph_keyword">Awake</span>, nó chỉ được gọi một lần duy nhất.</li></ul>



<p class="ph_question">“Hàm Start còn có gì khác so với Awake nữa không?”</p>



<p>Có một điểm đặc biệt của hàm <span class="ph_keyword">Awake</span>, đó là nó sẽ được gọi kể cả khi script KHÔNG được enable (xem ảnh dưới), trong khi <span class="ph_keyword">Start</span> thì sẽ không được gọi. Tuy nhiên trong trường hợp <span class="ph_keyword">GameObject</span> deactive thì không có hàm nào được gọi.</p>



<div class="wp-block-image"><figure class="aligncenter size-large"><img loading="lazy" width="562" height="52" src="https://phuongne.com/wp-content/uploads/2020/04/image-3.png" alt="checkbox disable enable monobehaviour" class="wp-image-696" srcset="https://phuongne.com/wp-content/uploads/2020/04/image-3.png 562w, https://phuongne.com/wp-content/uploads/2020/04/image-3-300x28.png 300w" sizes="(max-width: 562px) 100vw, 562px"><figcaption>Checkbox enable-disable script</figcaption></figure></div>



<p>Như vậy, các hàm thuộc loại <span class="ph_keyword">Initialization</span> thường được sử dụng để khởi tạo các giá trị có sẵn hoặc cache các components (<span class="ph_keyword">GetComponent</span>), trong đó chỉ có <span class="ph_keyword">OnEnable()</span> có thể được gọi nhiều lần</p>



<h2><span id="II_Game_Logic">II. Game Logic</span></h2>



<p>Ở phần này mình sẽ không đề cập về <strong>Internal Animation Update</strong>, ta chỉ quan tâm đến phần này khi sử dụng <span class="ph_keyword">StateMachineBehaviour</span>. <br>Đại loại nếu <span class="ph_keyword">MonoBehaviour</span> được gắn vào vào các GameObject thì <span class="ph_keyword">StateMachineBehaviour</span> sẽ được gắn vào các animation state và cũng có các hàm tương tự để xử lý</p>



<ul><li><strong>Update<em>:</em></strong> chắc hẳn hàm này đã quá quen thuộc khi chúng ta mới bắt đầu sử dụng Unity engine, <span class="ph_keyword">Update</span> được gọi mỗi lần vào mỗi frame và được xem như hàm xử lý chính của vòng lặp game.</li></ul>



<ul><li><strong>LateUpdate<em>:</em></strong> <span class="ph_keyword">LateUpdate()</span> được gọi như <span class="ph_keyword">Update</span>, mỗi frame một lần, điểm khác biệt duy nhất là nó được gọi sau khi các hàm <span class="ph_keyword">Update</span> của tất cả các <span class="ph_keyword">MonoBehaviour</span> đã được thực thi xong.</li></ul>



<p>Một chức năng kinh điển của hàm này là khi sử dụng camera follow theo player, sau khi vị trí cũng như rotation của player đã được tính toán hoàn tất trong <span class="ph_keyword">Update</span>, thì ta sẽ <span class="ph_keyword">LateUpdate</span> vị trí và góc xoay của camera theo player, đảm bảo được độ chính xác cao.</p>



<p><em>yield Null, WaitForSeconds, WWW, StartCoroutine</em>,… được thực thi tiếp khi sử dụng ở phần <span class="ph_keyword">Coroutine</span>, có thể đọc bài <a rel="noreferrer noopener" href="https://phuongne.com/coroutine-va-threads/" target="_blank">Coroutine trong Unity là gì?</a> để tham khảo thêm.</p>



<h2><span id="III_Physics">III. Physics</span></h2>



<ul><li><strong>FixedUpdate</strong>: Hàm này được gọi không phụ thuộc vào vòng lặp chính của game mà gọi theo vòng lặp của vật lý trong game, thường nó được gọi cố định vào mỗi 0.02s theo mặc định của project setting, con số này gọi là <span class="ph_keyword">Fixed Timestep</span> hay <span class="ph_keyword">fixedDeltaTime</span>.</li></ul>



<div class="wp-block-image"><figure class="aligncenter size-large"><img loading="lazy" width="439" height="189" src="https://phuongne.com/wp-content/uploads/2020/04/image-2.png" alt="" class="wp-image-694" srcset="https://phuongne.com/wp-content/uploads/2020/04/image-2.png 439w, https://phuongne.com/wp-content/uploads/2020/04/image-2-300x129.png 300w" sizes="(max-width: 439px) 100vw, 439px"><figcaption>Điều chỉnh Fixed Timestep trong Project Settings</figcaption></figure></div>



<p>Vì vậy <span class="ph_keyword">FixedUpdate</span> có thể được gọi nhiều hơn một lần hoặc không gọi trong 1 frame tùy theo FPS của game</p>



<ul><li><strong>Internal Physics Update:</strong> Đây là vùng xử lý chính của <span class="ph_keyword">Physics System</span> trong unity được xử lý riêng mà chúng ta không can thiệp, với một số chức năng sẵn có như áp trọng lực, trigger các hàm va chạm, di chuyển các vật thể sử dụng vật lý (rigidbody, joints,…)</li></ul>



<p>Vùng này được thực thi sau <span class="ph_keyword">FixedUpdate</span>, vì vậy các xử lý liên quan tới vật lý thì chúng ta nên đặt ở trong <span class="ph_keyword">FixedUpdate</span> thay vì <span class="ph_keyword">Update</span> để <span class="ph_keyword">Physics System</span> của Unity có thể cập nhật vị trí và xét va chạm kịp thời.</p>



<p>Mình đã nói qua vấn đề lỗi này ở bài <a rel="noreferrer noopener" href="https://phuongne.com/rigidbody-rigidbody2d/" target="_blank">Tui không hiểu gì về Rigidbody</a>.</p>



<h2><span id="IV_Decommissioning">IV. Decommissioning</span></h2>



<ul><li><strong>OnApplicationQuit</strong>: cái tên cũng nói lên được công dụng của hàm này rồi, nó sẽ được gọi trước khi thoát game (hoặc tắt <span class="ph_keyword">Play mode</span> trong <span class="ph_keyword">Unity Editor</span>)</li></ul>



<ul><li><strong>OnDisable:</strong> hàm này tương ứng với <span class="ph_keyword">OnEnable</span> mà mình đã đề cập ở trên, có thể được gọi nhiều lần nếu GameObject <span class="ph_keyword">active-deactive</span> nhiều lần (hoặc <span class="ph_keyword">enable-disable</span> Component gắn vào GameObject)</li></ul>



<ul><li><strong>OnDestroy:</strong> cuối cùng là <span class="ph_keyword">OnDestroy</span>, hàm này sẽ được gọi ở cuối frame, đồng nghĩa với việc khi xóa một <span class="ph_keyword">GameObject</span> trong scene (bằng script hoặc các sự kiện như thoát game, chuyển scene,…) hay sử dụng hàm <strong>Destroy(gameObject)</strong>, nó sẽ không xóa ngay lập tức mà phải đến cuối frame đó nó mới được dọn dẹp.</li></ul>



<p>Để dọn dẹp một <span class="ph_keyword">GameObject</span> ngay lập tức mà không cần delay tới cuối frame, có thể sử dụng <span class="ph_keyword">DestroyImmediate</span>, tuy nhiên Unity khuyến cáo là chỉ nên sử dụng khi debug và không nên sử dụng trong game.</p>



<h4><span id="Loi_ket">Lời kết</span></h4>



<p>Nếu các bạn thấy sai sót hay có ý kiến thì contact mình qua page hoặc comment phía bên dưới nhé</p>



<p>Nguồn tham khảo:</p>



<ul><li><a rel="noreferrer noopener" href="https://docs.unity3d.com/Manual/ExecutionOrder.html" target="_blank">Order of Execution for Event Functions</a></li></ul>
        <!-- </div> -->
          </div>
    
<div id="comments" class="comments-area">

  
  	<div id="respond" class="comment-respond">
		<h3 id="reply-title" class="comment-reply-title">Trả lời <small><a rel="nofollow" id="cancel-comment-reply-link" href="/awake-start-cac-ham-monobehaviour/#respond" style="display:none;">Hủy</a></small></h3><form action="https://phuongne.com/wp-comments-post.php" method="post" id="commentform" class="comment-form"><p class="comment-notes"><span id="email-notes">Email của bạn sẽ không được hiển thị công khai.</span> Các trường bắt buộc được đánh dấu <span class="required">*</span></p><p class="comment-form-comment"><label for="comment">Bình luận</label> <textarea id="comment" name="comment" cols="45" rows="8" maxlength="65525" required="required"></textarea></p><p class="comment-form-author"><label for="author">Tên <span class="required">*</span></label> <input id="author" name="author" type="text" value="" size="30" maxlength="245" required='required' /></p>
<p class="comment-form-email"><label for="email">Email <span class="required">*</span></label> <input id="email" name="email" type="text" value="" size="30" maxlength="100" aria-describedby="email-notes" required='required' /></p>
<p class="comment-form-url"><label for="url">Trang web</label> <input id="url" name="url" type="text" value="" size="30" maxlength="200" /></p>
<p class="form-submit"><input name="submit" type="submit" id="submit" class="submit" value="Phản hồi" /> <input type='hidden' name='comment_post_ID' value='610' id='comment_post_ID' />
<input type='hidden' name='comment_parent' id='comment_parent' value='0' />
</p></form>	</div><!-- #respond -->
	
</div><!-- #comments -->

  </section>

  <div class="sidebar f-grow1 f-basis4">
    <div id="search-4" class="widget widget_search"><h3>SEARCH</h3><form class="search-form" method="GET" action="https://phuongne.com/">
  <div class="search-form__group">
    <input class="search-form__s" type="search" name="s" id="search" placeholder="Search...">
    <!-- <input class="search-form__submit" type="submit" value="Search"> -->
    <button class="search-form__submit" type="submit" ><i class="fa fa-search"></i></button>
  </div>
</form></div>
		<div id="recent-posts-4" class="widget widget_recent_entries">
		<h3>LATEST POSTS</h3>
		<ul>
											<li>
					<a href="https://phuongne.com/serializefield-header-attribute-unity-p1/">SerializeField, Header và một số attributes trong Unity3D (P1)</a>
									</li>
											<li>
					<a href="https://phuongne.com/script-serialization-trong-unity3d/">Script Serialization trong Unity3D là gì?</a>
									</li>
											<li>
					<a href="https://phuongne.com/shader-trong-unity/">Shader 1 &#8211; Làm quen với Shader trong Unity</a>
									</li>
											<li>
					<a href="https://phuongne.com/awake-start-cac-ham-monobehaviour/" aria-current="page">Awake, Start và một số hàm cơ bản trong MonoBehaviour</a>
									</li>
											<li>
					<a href="https://phuongne.com/object-pooling-trong-unity/">Tối ưu với Object Pooling Pattern trong Unity</a>
									</li>
					</ul>

		</div><div id="categories-2" class="widget widget_categories"><h3>Categories</h3>
			<ul>
					<li class="cat-item cat-item-4"><a href="https://phuongne.com/category/c/">C#</a> (6)
</li>
	<li class="cat-item cat-item-5"><a href="https://phuongne.com/category/graphic/">Graphic</a> (6)
</li>
	<li class="cat-item cat-item-747"><a href="https://phuongne.com/category/optimizing/">Optimizing</a> (1)
</li>
	<li class="cat-item cat-item-6"><a href="https://phuongne.com/category/theory/">Theory</a> (9)
</li>
	<li class="cat-item cat-item-933"><a href="https://phuongne.com/category/tutorial/">Tutorial</a> (2)
</li>
	<li class="cat-item cat-item-1"><a href="https://phuongne.com/category/unity/">Unity</a> (15)
</li>
			</ul>

			</div><div id="text-2" class="widget widget_text">			<div class="textwidget"><p><a class="dmca-badge" title="DMCA.com Protection Status" href="//www.dmca.com/Protection/Status.aspx?ID=466766af-4a39-437b-987e-6f8d5e04b8a6"> <img src="https://images.dmca.com/Badges/dmca-badge-w150-5x1-06.png?ID=466766af-4a39-437b-987e-6f8d5e04b8a6" alt="DMCA.com Protection Status" /></a> <script src="https://images.dmca.com/Badges/DMCABadgeHelper.min.js"> </script></p>
</div>
		</div>  </div>

</div>

</main>

<footer class="site-footer">
  <h1><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="d989b1acb6b7beb7bc99ebe9ebe9">[email&#160;protected]</a></h1>
</footer>

<link rel='stylesheet' id='lwptoc-main-css'  href='https://phuongne.com/wp-content/plugins/luckywp-table-of-contents/front/assets/main.min.css?ver=2.1.4'  media='all' />
<script data-cfasync="false" src="/cdn-cgi/scripts/5c5dd728/cloudflare-static/email-decode.min.js"></script><script  async='async' src='https://phuongne.com/wp-content/themes/phuongne/assets/js/scripts-bundled.js?ver=1.0' id='phuongne-scripts-js'></script>
<script  async='async' src='https://phuongne.com/wp-includes/js/wp-embed.min.js?ver=5.6' id='wp-embed-js'></script>
<script  async='async' src='https://phuongne.com/wp-content/plugins/luckywp-table-of-contents/front/assets/main.min.js?ver=2.1.4' id='lwptoc-main-js'></script>
<style>.lwptoc .lwptoc_i A{color:#2b7abf;}.lwptoc .lwptoc_i A:hover,.lwptoc .lwptoc_i A:focus,.lwptoc .lwptoc_i A:active{color:#dd5858;border-color:#dd5858;}</style>
</div>
</body>

</html>
 
