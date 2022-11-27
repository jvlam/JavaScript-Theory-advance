# Scope
- Các phạm vi 
    - Global - toàn cầu (**tạo ra những biến hàm không nằm trong phạm vi code block và local scope**)
    - Code block - khối mã : let, const
    - Local scope - Hàm : var, function

    - Khi gọi mỗi hàm (hay hàm được thực thi) luôn có 1 phạm vi mới được tạo ra 
    - Các hàm có thể truy cập các biến được **khai báo trong phạm vi của nó** và **bên ngoài** nó
    - Cách thức một biến được truy cập
        + luôn tìm phạm vi gần nhất , nếu không có thì sẽ nhảy ra phạm vi bên ngoài, tìm không thấy báo lỗi
    - Khi nào một biến bị xóa khỏi bộ nhớ
        - **biến toàn cầu?**
            + Từ khi được khai báo biến global, giá trị sẽ được lưu trong bộ nhớ 
            + được xóa khi chương trình bị thoát , hay nhấn f5
            + note: HẠN CHẾ SỬ DỤNG BIẾN TOÀN CẦU , NẾU NHU CẦU SỬ DỤNG KHÔNG CAO SẼ BỊ TỐN BỘ NHỚ  
        - **biến trong code block trong hàm** 
            + biến và hàm khi thực thi xong trong block sẽ được engine tự động xóa khỏi bộ nhớ
            + In some programming languages, the local variables within a **function exist for just the duration** of that function's execution
        - **biến trong hàm được tham chiếu bởi 1 hàm**
            + vd: Scope.js

    - tưởng tượng như các hộp chứa nhau , hộp lớn nhất là global scope ,các hộp sau đó nhỏ dần
        + biến hay hàm được tạo ra ở hộp lớn hơn thì có thể truy cập được ở hộp nhỏ hơn
        + biến hay hàm được tạo ra ở hộp nhỏ hơn thì không thể truy cập được ở hộp lớn hơn
    