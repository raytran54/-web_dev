# TRAN CONG DANH - SVTT - Mentor: LUU VAN LAN - CSS - Day Started: 25/04/2024.
## Mục lục:
1.[ CSS Selector](#css-selector)

2.[ CSS Counter](#css-counter)

## CSS Selector
-CSS là gì: CSS là chữ viết tắt của Cascading Style Sheets, nó là một ngôn ngữ được sử dụng để tìm và định dạng lại các phần tử được tạo ra bởi các ngôn ngữ đánh dấu (HTML). Nói ngắn gọn hơn là ngôn ngữ tạo phong cách cho trang web. Bạn có thể hiểu đơn giản rằng, nếu HTML đóng vai trò định dạng các phần tử trên website như việc tạo ra các đoạn văn bản, các tiêu đề, bảng,…thì CSS sẽ giúp chúng ta có thể thêm style vào các phần tử HTML đó như đổi bố cục, màu sắc trang, đổi màu chữ, font chữ, thay đổi cấu trúc…

- Những chức năng đơn giản của CSS:
  
-CSS Selector:
+ The CSS element Selector : chọn các phần tử HTML dựa trên tên phần tử.
* Ví dụ:
```  
<!DOCTYPE html>
<html>
<head>
<style>
p {
  text-align: center;
  color: red;
} 
</style>
</head>
<body>

<p>Every paragraph will be affected by the style.</p>
<p id="para1">Me too!</p>
<p>And me!</p>

</body>
</html>
```
+ The CSS id Selector : sử dụng thuộc tính id của phần tử HTML để chọn một phần tử cụ thể. Id của một phần tử là duy nhất trong một trang, vì vậy bộ chọn id được sử dụng để chọn một phần tử duy nhất!

Để chọn một phần tử có id cụ thể, hãy viết ký tự băm (#), theo sau là id của phần tử.
* Ví dụ:
```
<!DOCTYPE html>
<html>
<head>
<style>
#para1 {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<p id="para1">Hello World!</p>
<p>This paragraph is not affected by the style.</p>

</body>
</html>
```
+ The CSS class Selector: chọn các phần tử HTML có thuộc tính lớp cụ thể. Để chọn các phần tử thuộc một lớp cụ thể, hãy viết ký tự dấu chấm (.), theo sau là tên lớp.
+  Ví dụ:
  ```
<!DOCTYPE html>
<html>
<head>
<style>
.center {
  text-align: center;
  color: red;
}
</style>
</head>
<body>

<h1 class="center">Red and center-aligned heading</h1>
<p class="center">Red and center-aligned paragraph.</p> 

</body>
</html>

```
## CSS Counter
-The CSS counter: là "các biến" được duy trì bởi CSS có giá trị có thể tăng lên theo quy tắc CSS (để theo dõi số lần chúng được sử dụng). Bộ đếm cho phép bạn điều chỉnh giao diện của nội dung dựa trên vị trí của nó trong tài liệu.

+ Để làm việc với CSS counter, chúng ta sẽ sử dụng các thuộc tính sau:
     * counter-reset: Tạo hoặc đặt lại bộ đếm
     * counter-increment: Tăng giá trị bộ đếm
     * content:  Chèn nội dung được tạo
     * Hàm counter() hoặc counters(): Thêm giá trị của bộ đếm vào một phần tử
+ Để sử dụng bộ đếm CSS, trước tiên nó phải được tạo bằng tính năng counter-reset.
+ Ví dụ:
  
```
  <!DOCTYPE html>
<html>
<head>
<style>
body {
  counter-reset: section;
}

h1 {
  counter-reset: subsection;
}

h1::before {
  counter-increment: section;
  content: "Section " counter(section) ". ";
}

h2::before {
  counter-increment: subsection;
  content: counter(section) "." counter(subsection) " ";
}
</style>
</head>
<body>


<h1>HTML/CSS Tutorials</h1>
<h2>HTML</h2>
<h2>CSS</h2>
<h2>Bootstrap</h2>
<h2>W3.CSS</h2>

<h1>Scripting Tutorials</h1>
<h2>JavaScript</h2>
<h2>jQuery</h2>
<h2>React</h2>

<h1>Programming Tutorials</h1>
<h2>Python</h2>
<h2>Java</h2>
<h2>C++</h2>

</body>
</html>
```




