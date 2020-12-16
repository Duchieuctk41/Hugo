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

### Bất đồng bộ là gì?
Là xử lý công việc không theo tuần tự, trong thời gian chờ làm việc này thì nhảy qua việc khác.

### Event loop là gì, Call stack là gì hoạt động như thế nào ?
Event Loop là cơ chế giúp Javascript có thể thực hiện nhiều thao tác cùng một lúc (concurrent model). 

Event Loop có một công việc đơn giản: theo dõi Call Stack và Callback Queue (hàng đợi các hàm callback). Nếu Call Stack đang trống, nó sẽ lấy event đầu tiên từ trong hàng đợi ra và đẩy nó vào trong Call Stack - tức là thực thi nó.

JavaScript là ngôn ngữ lập trình single-threaded.
Call stack là 1 cấu trúc dữ liệu, lưu các lệnh sẽ được thực thi. Vào sau thì ra trước.

### So sánh các cách xử lí của JS: callback, promise, async, await…

#### Callback (ES5)
Callback hiểu đơn giản là bạn truyền một hàm B vào hàm A dưới dạng 1 tham số, một lúc nào đó thì hàm A sẽ gọi hàm B để chạy. nhược điểm tạo ra callback hell.

#### Promise (ES6)
Là "lời hứa" đại diện cho giá trị chưa tồn tại và giá trị đó sẽ được trả về vào một thời gian trong tương lai.

#### Async / Await (ES7):
 Async được dùng để khai báo một hàm bất đồng bộ. Các hàm bất đồng bộ sẽ luôn trả về một giá trị. Việc sử dụng async chỉ đơn giản là ngụ ý rằng một lời hứa sẽ được trả lại và nếu một lời hứa không được trả lại, JavaScript sẽ tự động kết thúc nó.
 
Await làm cho JavaScript đợi cho đến khi promise trả về kết quả. 



