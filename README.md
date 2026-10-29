# YÊU CẦU ĐẦU RA

1. Quá trình đồng bộ dữ liệu

Khi em viết code xong và nhấn Ctrl + S, file sẽ được lưu vào ổ SSD của máy tính. Sau đó, phần mềm sẽ tự động đồng bộ file lên Cloud. Khi đồng bộ xong, file sẽ có dấu tích xanh.

Nếu máy tính mất mạng thì file vẫn còn ở máy. Khi có mạng trở lại, file sẽ được đồng bộ tiếp.

2. Sắp xếp thư mục trên Cloud
Cloud Drive
```

-- Code
   |-- StartupProject
       |-- src
       |-- package.json
       |-- package-lock.json

-- Docs
   |-- BaoCao.docx
   |-- HuongDan.docx

-- Assets
    |-- Anh
    |-- Icon
```


3. Cách xử lý node_modules

Thư mục node_modules có rất nhiều file nhỏ nên nếu đồng bộ hết sẽ làm máy chạy chậm và tốn dung lượng Cloud.

Em sẽ thêm node_modules/ vào file .gitignore và cài đặt phần mềm đồng bộ để bỏ qua thư mục này. Các file code và file package.json, package-lock.json vẫn được đồng bộ để khi cần có thể cài lại thư viện bằng lệnh npm install.

4. Sử dụng Files On-Demand

Em bật Files On-Demand để không phải tải tất cả file trên Cloud về máy. File nào cần dùng thường xuyên thì giữ trên máy, file ít dùng thì để trên Cloud. Khi cần sử dụng, em có thể tải file đó về.
