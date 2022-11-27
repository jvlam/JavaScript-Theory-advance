# khái niệm
- **bind** là ràng buộc, sẽ giúp ràng buộc từ khóa [this] trong hàm trong các phương thức, trở thành một đối tượng khác tùy ý

# đặc tính
- phương thức bind() sẽ trả về một hàm mới
- có thể nhận các đối số như hàm ban đầu

# đối số
- nhận vào một đối số đầu tiên: là object muốn ràng buộc nó với từ khóa [this] đối với method
- những đối số phía sau là tham số của function mà bind() ràng buộc, tùy vào số lượng tham số function được bind() , tùy đối số của bind()
- sẽ có bấy nhiêu parameter

```js
bind(object, parameter1, parameter2, para ....)
```

- [bind()] làm việc với [function] , [method]

