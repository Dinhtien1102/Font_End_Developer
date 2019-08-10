# Fontend Deverloper
#### Nơi ghi ra những Kinh Nghiệm về Javascript, Css, HTML, Thư viện, Frameworks, Github... 1 vài công cụ công nghệ code (visua code)... thậm trí là liệt kê các nguồn tài liệu hay
***
- **[Github & Git](#github-and-git)**
- **[HTML Advanced](#html-advanced)**
- **[CSS Advanced](#css-advanced)**
- **[Responsive](#Responsive)**
- **[Javascipt](#javascript)**
- **[How To](#how-to)**
- **[ReactJS](#reactjs)**
- **[Vue.JS](#vuejs)**
***
## Github and Git
- [Shields IO](https://shields.io/?fbclid=IwAR3GPWdASNiGAkf21bJXXy2UnmJUCBkb6NXu_JnBv-uOBEaYInycfTSzMeA)
```
- git revert 23f3e289c44d7ab0b136 : dùng để lấy lại tại id commit : 23f3e289c44d7ab0b136
- git reset 23f3e289c44d7ab0b136 : dùng để khôi phục tất cả file của các dự án sau liền kề id commit: 23f3e289c44d7ab0b136
- git add . : dùng để đánh dấu toàn bộ file dự án
- git commit : dùng để chú thích cho mỗi lần thay đổi dự án 
- git pull : dùng để tải dự án về
- git push : dùng để đẩy một dự án lên
- Bắt đầu 1 project: Tạo 1 kho trên github, sau đó tạo file READEME.md tại máy chủ và push dự án
- Xác thực khóa: $ eval $(ssh-agent)
                 $ ssh-add ../Dinhtien1102
```
### tạo kho git và file README.md trên web git
- copy mã clone tại Clone with HTTPS 
- vào visual mở foder cần tải lên github
- mở git bash
- dòng đầu: git clone + mã HTTPS 
=> đã tải xong kho git về máy chủ của bạn
- mở foder chứa file bạn cần đưa lên github, copy tất cả file đó paste vào kho bạn vừa clone thành một foder
- tiếp tục vào visual mở foder có chứa kho và các file đó
=> mở git git bash
- dòng đầu : git add .
- `git commit -m "..."`
- `git push`
==> Giờ thì vào kiểm tra Kho của bạn đã up dự án thành công chưa :)
#### ĐỂ TÌM 1 KHO TRÊN GITHUB ĐÃ TẢI VÊ TẠI LOCAL NÀO => VÀO Ổ C => USER => ADMIN
***
## HTML Advanced
  - [Thêm viền text_StrokeText](https://css-tricks.com/adding-stroke-to-web-text/) (-webkit-text-stroke: 1px black;)
***
##  Css Advanced
- Sử dùng border bị đẩy khối: trường hợp dùng thuộc tính border khi hover trong list menu và các khối đẩy nhau
```css
    a {
    border: 1px solid transparent;
    }
    a:hover {
    background-color: #EBF6FD;
    border: 1px solid #dcf0fb;
    }
- Gradient button
```css
   .button {
   width: 200px;
   height: 100px;
   background-size: 200% auto;
   transition: 0.5s;
   background-image: linear-gradient(to right, #314755 0%, #26a0da 51%, #314755 100%)
   }
   .button:hover { 
    background-position: right center; 
    }
```
+ CSS Loader

+ Style HR

+ Color value: #rgb, #rrggbb, hsl(hue, saturation, lightness)

+ Background:
   - `background-repeat: repeat-x(hoặc y)` Lặp lại hình ảnh theo chiều ngang (hoặc dọc) 
   - `background-repeat: no-repeat` Background-image không lặp lại 
   - `background-poisition: giá trị` Thay đổi vị trí của hình ảnh 
   - `background-attachment: fixed` Chỉ định hình nền sẽ không cuộn với phần còn lại của trang
   - Rút ngắn mã có thể đặt các giá trị trên vào thuộc tính 
        -`Background: value(background-color, background-image, background-repeat, background-attachment, background-position)`.
      
      
 + Transition: 
    - sử dụng display: none => không hiển thị (transition không hiển thị)
    ```css 
           #spinner-success-text {
            display: none;
            transition: all 1s ease-in;
            }
           #spinner-success-text.show {
            display: block;
            }
     ```
     - thay vào đó hãy dùng opacity => vấn đề transition đã được giải quyết
     ``` css
          #spinner-success-text {
          opacity: 0;
          transition: all 1s ease-in;
          }
          #spinner-success-text.show {
              opacity: 1;
          }
      ```
+ thay đổi con trỏ với hình ảnh
cursor : -webkit-image-set(url(/img/obj-cursor-right.png) 1x,url(/img/obj-cursor-right@2x.png) 2x),e-resize;

+ dùng transition để chuyển các slider mượt mà hơn vấn đề là khi click lần đầu thì transition không hoạt động nhưng lần 2 và nhiều         lần sau lại được **cần xác định vị trí khối ta muốn thêm thuộc tính transition (Đối với khối đã có position thì xác định top, bottom, left, right; với các khối còn lại ta sử dụng margin-top, margin-left, margin-bottom, margin-right để xác định vị trí cho khối đó)**
+ scroll-behavior: smooth;  
## Responsive
  + Text
  
## Javascript
#### Chú ý:
   - tong = tong + a *đối với phép gán thì biến bên trái chỉ được gọi ra và ko được xử lí, còn bên phải là giá trị gán cho biến đó để thực phép toán*
   - if(tong + 1 == tong + a) *Đối với phép bằng thì cả 2 biến đều cùng thực hiên phép toán*
   
  #### Variables (Biến và kiểu dữ liệu trong Javascript)
  + Các biến javascript là các thùng chứa gái trị dữ liệu
  + Let, var, khai báo hằng số const
  + Các kiểu dữ liệu: 
      - Numbers
      - Strings
      - Booleans: True & False
      - Array
      - Object
  #### Operator   
  [Toán Tử](https://developer.mozilla.org/vi/docs/Web/JavaScript/Guide/Expressions_and_Operators)
  ##### JavaScript Arithmetic Operators
  | Operator    | Description     |
  | ----------- | ----------------|
  |+            | Addition        |
  | -           | Subtraction     | 
  | *           | Multiplication  | 
  |**           |	Exponentiation  |
  | /           | Division        | 
  | %           | Chia lấy dư     | 
  | ++          | Increment       | 
  | --          | Decrement       | 
      
  #### Object (Đối Tượng) trong Javascript
   + Các giá trị được lưu dưới dạng *name: value* trong đó name: thuộc tính, value: giá trị thuộc tính
   + Giá trị thùng chứa javascript là các thùng chứa cho các giá trị được gọi là các thuộc tính hoặc phương thức, mỗi thuộc tính được ngăn cách bởi dấu "," 
   + Truy cập thuộc tính đối tượng (Accessing Object Properties)
        - Cách 1: objectName.propertyName
        - Cách 2: objectName["propertyName"]
   + Object Methods 
   
  #### String(Chuỗi)-Object đặc biệt
  ##### Chú ý: 
   + Có thể là 0 hoặc nhiều kí tự được viết bên trong "" hoặc ''
   + Có thể sử dụng dấu '' hoặc "" bên trong chuỗi
   + String Lenght
      - nameString.lenght
   
  #### Array(Mảng)- Cách chứa nhiều giá trị
  #### Control Statement(Câu lệnh điều khiển)- If-Else/Switch-Case
  #### Vòng Lặp(Loop)-For, For-of, While
  #### Hàm (Function)- Tách chương trình thành nhiều phần
  #### Dom
  #### Event 
  #### Ajax
  #### ES6
## How To

  + Flip Card
  
  + Popover

  + Dialog

  + Tooltip

  + Popup

  + Collapse
  
  + Overlay
  
  + Alerts
  
  + Cutout Text

  + Timeline

  + Scroll Indicator

  + Range Sliders
  
  + Create a To Do List

## ReactJS
## VueJS
