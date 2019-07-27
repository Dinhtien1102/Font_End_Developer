# Fontend Deverloper
#### Nơi ghi ra những Kinh Nghiệm về Javascript, Css, HTML, Thư viện, Frameworks, Github... 1 vài công cụ công nghệ code (visual code)... thậm trí là liệt kê các nguồn tài liệu hay
***
## Github
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
##  Css Advanced

+ Color value: #rgb, #rrggbb, hsl(hue, saturation, lightness)

+ Background:
   - `background-repeat: repeat-x(hoặc y)` Lặp lại hình ảnh theo chiều ngang (hoặc dọc) 
   - `background-repeat: no-repeat` Background-image không lặp lại 
   - `background-poisition: giá trị` Thay đổi vị trí của hình ảnh 
   - `background-attachment: fixed` Chỉ định hình nền sẽ không cuộn với phần còn lại của trang
   - `Background: value(background-color, background-image, background-repeat, background-attachment, background-position)`.
      Rút ngắn mã có thể đặt các giá trị trên vào thuộc tính 
   - `background-color`
   - `background-image` 
   
 + Transition: 
    ```css sử dụng display: none => không hiển thị (transition không hiển thị)
           #spinner-success-text {
            display: none;
            transition: all 1s ease-in;
            }
           #spinner-success-text.show {
            display: block;
            }
     ```
     ``` thay vào đó hãy dùng opacity => vấn đề transition đã được giải quyết
          #spinner-success-text {
          opacity: 0;
          transition: all 1s ease-in;
          }
          #spinner-success-text.show {
              opacity: 1;
          }
      ```
