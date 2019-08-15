
##  Css Advanced
- [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
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
- style button https://desktop.github.com/
``` css
    .button {
        background-image: linear-gradient(to bottom, #8241f9, #4e277b);
        border-color: #150a27;
        color: #fff;
        background-repeat: repeat-x;
        background-position: -1px -1px;
        background-size: 110% 110%;
        border: 1px solid rgba(27,31,35,0.2);
        border-radius: 0.25em;
        }
    
    .button:hover {
        background: none;
        background-image: linear-gradient(to bottom, #8c50f9, #552b87);
        border-color: #150a27;
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
- Các đường sọc chéo chạy trong 1 khối
[Sọc Chéo Animation](https://codepen.io/KingkongVN99/pen/PoYNJPZ)
![Animation](https://raw.githubusercontent.com/Dinhtien1102/Fontend_Developer/master/img/animation.PNG)
``` css
@keyframes animation-15lk19q {
    0%{background-position:0 0;}
    100%{background-position:2rem 4rem;}
}
.background {
    height: 300px;
    -webkit-align-items: center;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    background-color: #663399;
    cursor: pointer;
    -webkit-flex-shrink: 0;
    -ms-flex-negative: 0;
    flex-shrink: 0;
    line-height: 1.25;
    -webkit-text-decoration: none;
    -webkit-font-smoothing: antialiased;
    background-size: 2rem 2rem;
    -webkit-transition: all 250ms cubic-bezier(0.4,0,0.2,1);
    transition: all 250ms cubic-bezier(0.4,0,0.2,1);
}

.background:hover {
    background-color: #663399;
    background-image: linear-gradient(135deg,rgba(0,0,0,0.1) 25%,transparent 25%,transparent 50%,rgba(0,0,0,0.1) 50%,rgba(0,0,0,0.1) 75%,transparent 75%,transparent);
    color: #ffffff;
    -webkit-animation: animation-15lk19q 2.8s linear infinite;
    animation: animation-15lk19q 2.8s linear infinite;
    border-color: #663399;
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
+ Làm màu ảnh => đen trắng và hover ảnh => màu ban đầu
``` css
    .img:hover {
        -webkit-filter: grayscale(0);
        filter: grayscale(0);
        }
    .img {
        -webkit-filter: grayscale(1);
        filter: grayscale(1);
        -webkit-transition: all 0.4s;
        }
 ```

+ thay đổi con trỏ với hình ảnh
cursor : -webkit-image-set(url(/img/obj-cursor-right.png) 1x,url(/img/obj-cursor-right@2x.png) 2x),e-resize;

+ dùng transition để chuyển các slider mượt mà hơn vấn đề là khi click lần đầu thì transition không hoạt động nhưng lần 2 và nhiều         lần sau lại được **cần xác định vị trí khối ta muốn thêm thuộc tính transition (Đối với khối đã có position thì xác định top, bottom, left, right; với các khối còn lại ta sử dụng margin-top, margin-left, margin-bottom, margin-right để xác định vị trí cho khối đó)**
+ scroll-behavior: smooth;  
## Responsive
  + Text
*** 
