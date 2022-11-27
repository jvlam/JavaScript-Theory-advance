# Closure (tính khép kín , tính bao đóng của hàm trong js)

- Là một hàm có thể **ghi nhớ nơi nó được tạo** ra và **truy cập được biến ở bên ngoài phạm vi** của nó  - a Sơn

- a closure gives you access to an **outer function's scope** from an **inner function**  - mozilla
- In JavaScript, closures are created every time a function is created, at function creation time. - mozilla

# lexical scoping 
    - khi mà một function được khởi tạo trong phạm vi của một parent's function, nhưng lại có thể truy cập được biến của
    phạm phi parent's function thì đó gọi là **lexical scoping**.

## Ứng dụng
- Viết code ngắn gọn hơn 
- Biểu diễn , ứng dụng tính Private trong OOP 


# lưu ý
    - Biến được tham chiếu (refer) trong closure sẽ không được xóa khỏi bộ nhớ khi hàm cha thực thi xong
    - nó sẽ bị xóa khỏi bộ nhớ khi closure thực thi xong


**note:** tính khép kín, sự bao đóng --> mỗi một function khi được gọi sẽ tạo ra một môi trường thực thi riêng biệt 
                                         do đó mỗi lần khai báo một biến or một function con nằm trong một hàm cha 
                                         thì bên ngoài hàm cha đó không thể truy cập được vào các biến và các hàm bên trong
          --> do tính chất đó người ta mới khái quoát hóa gọi là **closure**         