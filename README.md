# TRAN CONG DANH - SVTT - Mentor: LUU VAN LAN - HTML co ban - Day Started: 22/04/2024.
## Mục lục:
1. [Tổng quan](#tổng-quan)
2. [Tag heading](#tag-heading)
3. [Tag link](#tag-link)
4. [Tag Image](#tag-image)

 ## Tổng quan
-Tài liệu HTML phải được khai báo dưới dạng: <!DOCTYPE html> và chính html document cũng phải bắt đầu bằng <html> và kết thúc bằng </html>. Phần tiếp đến là cặp <body></body> nơi chứa các tag và script liên quan. 
   + Một ví dụ về html đơn giản:
     ```
        < !DOCTYPE html>

        < html>
  
        < body> 
  
        < h1 >My First Heading< /h1>
  
        < p >My first paragraph.< /p>
  
        < /body>
  
        < /html>
## Tag heading  
-HTML heading: được định nghĩa với các tag từ < h1 > đến < h6 >. < h1 > được định nghĩa là quan trọng nhất, < h6 > ít quan trọng nhất.
## Tag link
-HTML Links: được định nghĩa với tag < a >.

  +Ví dụ: 
      
      < !DOCTYPE html>
   
      < html>
     
      < body>
     
      <a href="www.google.com" > This is a valid link </a>
    
      < /html>
     
      < /body>
## Tag image     
-HTML Images: được định nghĩa với tag <image> </image>. Source file được định nghĩa bằng (src), text thay thế (alt), (width) và (height) được cung cấp như là một attribute.

   +Ví dụ: < img src="pic.jpg" alt="Đây là tấm ảnh về HPT" width="100" height="100">
   + src attribute có 2 cách để trỏ đến file ảnh:
      * Đường dẫn chính xác - là đường link cho file ảnh ngoài được host bởi website khác. Ví dụ src="https://www.w3schools.com/images/img_girl.jpg".
      * Đường dẫn tương đối - là đường link mà file ảnh được host trong chính website. Ở đó URL sẽ không cần bao gồm domain. Nếu URL bắt đầu mà không có một dấu "/" nó sẽ liên quan đến trang hiện tại. Ví dụ: src="img_girl.jpg". Nếu URL bắt đầu bằng dấu "/", nó sẽ liên quan đến cái domain của website. Ví dụ: src="/images/img_girl.jpg". 
