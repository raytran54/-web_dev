# TRAN CONG DANH - SVTT - Mentor: LUU VAN LAN - HTML5 - Day Started: 24/04/2024.
## Mục lục:
1.[ Điểm mới](#điểm-mới)

2.[ HTML5-Events](#html5-events)

3.[ HTML5-SVG](#html5-svg)

4.[ HTML5-Web-Storage](#html5-web-strorage)

## Điểm mới
Phiên bản HTML5 đã cập nhật rất nhiều thẻ mới cho việc tạo lập các bài viết và đa phương tiện, điển hình là các thẻ sau:

   < article>: Định nghĩa một bài viết hoặc bình luận của người dùng, độc lập với content của website.
  
   < aside>: Đánh dấu nội dung một trang hiện tại.
  
   < header>< footer>: Loại bỏ việc định nghĩa id cho tiêu đề và cuối trang.
  
   < nav>: Định nghĩa phần menu điều hướng cho website.
  
   < section>: Xác định các thành phần khác nhau trong website.
  
   < audio>, < video>: Hỗ trợ người dùng xem clip và nghe nhạc trên website mà không cần bên thứ ba.

   < embed>: Xác định một container các plugin tương tác với ứng dụng bên ngoài.

   < canvas>: Cho phép bạn đồ họa mà không cần ứng dụng hỗ trợ.

## HTML5-Events
Vậy, events là gì?
- Khi người dùng truy cập trang web, họ thực hiện nhiều hoạt động khác nhau như nhấp vào văn bản, hình ảnh và liên kết, di chuột qua các phần tử đã xác định, v.v. Đây là những ví dụ về những gì JavaScript gọi (events).
- 
  Những ví dụ về events:
  
offline	script	Triggers when the document goes offline

onabort	:	Triggers on an abort event

onafterprint	:	Triggers after the document is printed

onbeforeonload	:	Triggers before the document loads

onbeforeprint	:	Triggers before the document is printed

onblur	:	Triggers when the window loses focus

oncanplay	:	Triggers when media can start play, but might has to stop for buffering

oncanplaythrough	:	Triggers when media can be played to the end, without stopping for buffering

onchange	:	Triggers when an element changes

onclick	:	Triggers on a mouse click

oncontextmenu	:	Triggers when a context menu is triggered

ondblclick	:	Triggers on a mouse double-click

ondrag	:	Triggers when an element is dragged

ondragend	:	Triggers at the end of a drag operation

ondragenter	:	Triggers when an element has been dragged to a valid drop target

ondragleave	:	Triggers when an element leaves a valid drop target

ondragover	:	Triggers when an element is being dragged over a valid drop target

ondragstart	:	Triggers at the start of a drag operation

ondrop	:	Triggers when dragged element is being dropped

ondurationchange	:	Triggers when the length of the media is changed

onemptied	:	Triggers when a media resource element suddenly becomes empty

onended	:	Triggers when media has reach the end

onerror	:	Triggers when an error occur

onfocus	:	Triggers when the window gets focus

onformchange	:	Triggers when a form changes

onforminput	:	Triggers when a form gets user input

onhaschange	:	Triggers when the document has change

oninput	:	Triggers when an element gets user input

oninvalid	:	Triggers when an element is invalid

onkeydown	:	Triggers when a key is pressed

onkeypress	:	Triggers when a key is pressed and released

onkeyup	:	Triggers when a key is released

onload	:	Triggers when the document loads

+ Ví dụ sử dụng event autofocus để gửi 1 email đơn giản :

```
<!DOCTYPE HTML>

<html>
   <body>
   
      <form action = "/cgi-bin/html5.cgi" method = "get">
         Enter email : <input type = "text" name = "newinput" autofocus/>
         <p>Try to submit using Submit button</p>
         <input type = "submit" value = "submit" />
      </form>
      
   </body>
</html>
```
## HTML5-SVG

- SVG là viết tắt của Đồ họa vectơ có thể mở rộng và nó là ngôn ngữ để mô tả các ứng dụng đồ họa và đồ họa 2D trong XML và sau đó XML được hiển thị bởi trình xem SVG.

- SVG chủ yếu hữu ích cho các sơ đồ loại vectơ như biểu đồ Pie, đồ thị hai chiều trong hệ tọa độ X, Y, v.v.
+ Ví dụ:

  ```
  <!DOCTYPE html>

  <html>
   <head>
   
      <style>
         #svgelem {
            position: relative;
            left: 50%;
            -webkit-transform: translateX(-20%);
            -ms-transform: translateX(-20%);
            transform: translateX(-20%);
         }
      </style>
      <title>SVG</title>
      <meta charset = "utf-8" />
   </head>
   
   <body>
      <h2 align = "center">HTML5 SVG Circle</h2>
     <svg id = "svgelem" height = "200" xmlns = "http://www.w3.org/2000/svg">
         <circle id = "redcircle" cx = "50" cy = "50" r = "50" fill = "red" />
      </svg>
   </body>
  </html>
  ```
  ## HTML5-Web-Storage
- Có 2 loại Web Storage:
 
+Session Storage: Có thể thực hiện nhiều phiên giao dịch đơn trong nhiều của sổ trong cùng 1 trang web nhưng không ảnh hưởng đến nhau.
  
+Local Storage: Tương tự như session storage, nhưng chỉ khác một điều rằng:
  
   Tất cả thông tin, data của session storage sẽ bị mất khi đóng tab or trình duyệt.
  
   Local storage chỉ mất data khi người dùng xóa chúng khỏi máy.

+Ví dụ về Session Storage:
  ```
  <!DOCTYPE HTML>

  <html>
   <body>
      <script type = "text/javascript">
         
         if( sessionStorage.hits ) {
            sessionStorage.hits = Number(sessionStorage.hits) +1;
         } else {
            sessionStorage.hits = 1;
         }
         document.write("Total Hits :" + sessionStorage.hits );
      </script>
	
      <p>Refresh the page to increase the number of hits.</p>
      <p>Close the window and open it again and we find that the number of hits is returned to 1.</p>

    </body>
    </html>

+Ví dụ về Local Storage:

```
    <!DOCTYPE HTML>

    <html>
    <body>
      <script type = "text/javascript">
         
         if( localStorage.hits ) {
            localStorage.hits = Number(localStorage.hits) +1;
         } else {
            localStorage.hits = 1;
         }
         document.write("Total Hits :" + localStorage.hits );
      </script>
		
      <p>Refresh the page to increase the number of hits.</p>
      <p>Close the window and open it again and the number of hits is still the same as the last time that was shown on screen.</p>

   </body>
</html>
	
    

