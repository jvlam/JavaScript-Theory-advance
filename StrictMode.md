# khái niệm - ra đời phiên bản ES6
- chế độ nghiêm ngặt , một chế độ giúp code javascript chở nên an toàn hơn 

- khai báo biến mà sơ suất quên từ khóa **let**, **var**, **const** 
- một biến global sẽ giải phóng khi chương trình ngừng lại, đây có thể là một vấn đề tiềm ẩn gây những trường hợp rò rỉ bộ nhớ cho app
  hoặc lỗi logic tiềm ẩn do trùng với giá trị nào đó ở phạm vi global

=> do đó strict mode ra đời để khắc phục tình trạng này

# Cách sử dụng
- 1. thêm "use strict"; vào đầu file .js
- 2. thêm "use strict"; vào sau ngay thẻ mở <script>
- 3. thêm "use strict"; vào đầu phạm vi hàm 


# Công Dụng
    1. Tránh "quên" từ khóa khai báo biến
    2. Tránh trùng tên biến dẫn tới lỗi logic
    3. sử dụng bộ nhớ hiệu quả vì tránh tạo biến global
