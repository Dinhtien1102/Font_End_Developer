
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
 ```
    
- Gradient button: di chuyển màu sắc trong 1 khối
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
*** 
