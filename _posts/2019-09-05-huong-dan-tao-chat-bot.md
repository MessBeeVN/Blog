---
layout: post
title:  "How to Create a Chatbot - Part 1"
author: messbeevn
categories: [Hướng Dẫn]
image: assets/images/chatbot.png
---
Chào các bạn!

Chắc hẳn các bạn không còn xa lạ gì với Chatbot nữa, hiện nay để tạo một Chatbot cũng khá đơn giản nếu sử dụng qua một số app của bên thứ 3.

Vì vậy, hôm nay chúng tôi sẽ hướng dẫn các bạn cách làm thế nào để có thể xây dựng một hệ thống Chatbot Facebook Messenger cho riêng mình.

Để bắt đầu các bạn cùng xem hướng dẫn dưới đây nhé: 

**Bước 1. Cài đặt môi trường**

1. Các bạn tải Visual Studio Code (VSC) tại trang <https://code.visualstudio.com>
2. Node, NPM => <https://nodejs.org>
3. Sau khi cài đặt xong các bạn mở cmd kiểm tra nhé!
    - npm -v
    - node -v

**Bước 2. Khởi tạo dữ liệu**

1. Tạo thư mục lưu trữ code (**D:\Source\Repos\Chatbot**), mở VSC lên, open folder vừa tạo.
2. Khởi tạo một ứng dụng mới: **Mở Terminal (Ctrl+`)**, chạy lệnh ***npm init*** sau đó khai báo thông tin App.
3. Cài đặt Express bằng lệnh: ***npm install express*** --save
4. Tạo file **app.js** hoặc tên tuỳ ý (*mặc định là index.js*), thêm đoạn code sau vào file vừa tạo: 

        var express = require("express");
        var app = express();
        app.listen(3000, () => {
                console.log("Server running on port 3000");
        });
        app.get("/api/getNumbers", (req, res, next) => 
        {
                res.json([0,1,2,3,4,5,6,7,8,9]);
        });

5. Chạy app bằng lệnh: **node app.js**, mở đường dẫn <http://localhost:3000/api/getNumbers> kiểm tra kết quả.

Để xem video chi tiết các bạn xem [Tại Đây](https://www.youtube.com/watch?reload=9&v=5zE-tevfJbY&fbclid=IwAR3bYdHrMV-zAawvQnJ8gLDy-XtqDG5J20d853pzD5UKjMvGFWzyU4sAIHM).