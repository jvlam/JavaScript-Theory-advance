# khái niệm
- các nhóm kiểu dữ liệu trong js, nó thể hiện khi mà gán một biến thì dữ liệu đó được lưu trữ như thế nào trong bộ nhớ

# 1. Value types (primitive data types)
    - String 
    - Number 
    - Boolean
    - BigInt                                 `stack save` -> static memory allocation
    - Symbol                                  - engine knows the size at compile time -> the size won't change (at least 4 bytes or 8 bytes)
    - undefined                               - include primitive values and references(point to objects, function, array)
    - null          

# 2. Reference types (Non-primitive data types)
    - Object                                 `heap save` -> dynamic memory allocation
    - Array                                   - store object, function, array
    - Function                                - does not allocate fixed amount of memory, allocate more if needed 

## Data types with functions
    - Value types 
    - Reference types


# 3. Memory life cycle
    Regardless of the programming language, the memory life cycle is pretty much always the same:
        1. Allocate the memory you need
        2. Use the allocated memory (read, write)
        3. Release the allocated memory when it is not needed anymore


```js
let user = {
    name: 'Vũ Anh Lãm',
    age: 20,
    address: 'Hà Nội'
}

let userB = user;

user.address = 'Hồ Chí Minh'

console.log(user);
console.log(userB);
```
![This is an image](https://scontent.fsgn2-5.fna.fbcdn.net/v/t1.15752-9/315520873_459178496364399_4974682022744269445_n.png?_nc_cat=104&ccb=1-7&_nc_sid=ae9488&_nc_ohc=9q0QxOw79b4AX_vQwGD&tn=vvaCJEQmHGpOdMjY&_nc_ht=scontent.fsgn2-5.fna&oh=03_AdR1anxIT6YHscVG4pXPOSr7tVF6uhc4qBUa5OeFkGc43A&oe=63A94720)



![This is an image](https://scontent.fsgn2-5.fna.fbcdn.net/v/t1.15752-9/315004000_439748548339153_2723041057483088549_n.png?_nc_cat=106&ccb=1-7&_nc_sid=ae9488&_nc_ohc=5j5b2z_RAHgAX8ASaMq&_nc_ht=scontent.fsgn2-5.fna&oh=03_AdR1a_7nl_oX4VPO3L_cjgBX1bFytrLRapM56rch4SmAVw&oe=63A94701)
