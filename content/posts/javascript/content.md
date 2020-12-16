### Có 9 kiểu dữ liệu trong Javascript:

##### 6 kiểu Dữ liệu sơ khai (primitive), có thể kiểm tra với toán tử typeof:

Kiểu undefined 

Kiểu Boolean

Kiểu số

Kiểu chuỗi

Kiểu số BigInt 

Kiểu Symbol
 
Kiểu null: typeof instance === "object". 

Object: typeof instance === "object".

Phi dữ liệu Function instance === "function". 

### null : 
trả về object, và rỗng.
### underfined : 
giá trị không xác định

### var: 
Kiểu cũ, trc ES6: khai báo biến kiểu cũ có scope là  globally scoped. trừ var nằm trong hàm (scope là function/locally scoped). 

var dễ gây hoisting: dù khai báo ở đâu biến vấn bị đưa lên đầu hàng.
 
### let: 
Thay thế cho var, scope là block scope.
### const: 
Khai báo hằng.

### Scope
Là phạm vi truy cập: global, local

 ### Closure
Lexical global: hàm trong hàm, hàm con có quyền truy cập đến phạm vi biến của hàm cha.

Khái niệm closure bao đóng. làm cho scope trong không thể tiếp cận được public scope. Chỉ gọi function sẽ không thực hiện gì bởi nó trả về kết quả là tham chiếu tới function.


