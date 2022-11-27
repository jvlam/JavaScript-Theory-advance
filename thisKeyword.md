# khái niệm
- Trong hầu hết mọi trường hợp dùng từ khóa [this], từ khóa [this] sẽ trỏ về **đối tượng** mà nó đang thuộc về  (đối tượng trước dấu chấm)
- Đứng ngoài **phương thức** , [this] tham chiếu tới đối tượng Global Context 

- mỗi một function trong javaScript đều có một ngữ cảnh (Context = this) để chạy riêng (môi trường để chạy)

# note:
- [this] trong hàm tạo là đại diện cho đối tượng sẽ được tạo (nghĩa là nó có thể trỏ được đến đối tượng khác khi mà đối tượng được khởi tạo)
- [this] trong một hàm là **undefined** khi ở **strict mode** 
- các phương thức **bind()**, **call()**, **apply()** có thể tham chiếu [this] tới đối tượng khác 


- bản thân từ khóa [this] không phải là một biến mang giá trị, mà chỉ là một từ khóa tham chiếu đến đối tượng khác.
- **method** - một hàm được sử dụng làm thuộc tính của một Object, thì gọi là phương thức hay method

# cô đọng
- khi gọi hàm không thông qua một đối tượng, thì từ khóa [this] sẽ trỏ ra đối tượng global, và trình duyệt sẽ chọc ra phạm  vi window
    + ở trong chế độ **"strict mode"** thì sẽ bị undefined
- khi gọi hàm có object chấm ở trước sẽ, thì từ khóa [this] sẽ trỏ về đúng đối tượng được chấm