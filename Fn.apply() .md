# cách dùng
- tương tự như call() , nhưng đối số nhận vào là một mảng


# so sánh sự khác nhau giữa 3 phương thức 
- [bind()]
- [call()]
- [apply()]

# giống nhau
- đều kế thừa Function.prototype

```js
fn.bind === Function.prototype.bind // true
fn. call === Function.prototype. call // true
fn.apply === Function.prototype.apply // true
```

# khác nhau
- Các đối số & cách hoạt động 

```js
funcion fn() {} 

// Bind method
/* 
- trả ra hàm mới với `this` tham chiếu tới `thisArg`
- không thực hiện gọi hàm
- Nếu được bind kèm `arg1, arg2, ... ` thì các đối số này ưu tiên hơn 
*/
const newFun = fn.bind(thisArg, arg1, arg2, ...)

newFun(arg1, arg2, ...) // và gọi hàm mới 


//Call method
/*
   - Thực hiện bind `this` với `thisArg` và thực hiện gọi hàm
   - Nhận các đối số cho hàm gốc từ `argl, arg2, ... ...`
*/
fn. call(thisArg, arg1, arg2, ...)


//Apply method
/*
   - Thực hiện bind `this` với `thisArg` và thực hiện gọi hàm
   - Nhận các đối số cho hàm gốc bằng đối số thứ 2 dưới dạng mảng `[arg1, arg2, ...]`
*/
fn.apply(thisArg, [arg1, arg2, ...])


```