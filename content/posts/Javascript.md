---
title: "JavaScript"
date: 2020-12-15T03:18:36+07:00
---

#### #1 Javascript là gì ?

Javascript là ngôn ngữ lập trình thông dịch.

---

#### #2 Các kiểu dữ liệu trong Javascript ?

Có 9 kiểu dữ liệu trong Javascript:

6 kiểu Dữ liệu sơ khai (primitive), có thể kiểm tra với toán tử typeof:
Kiểu undefined, Kiểu Boolean, Kiểu số, Kiểu chuỗi, Kiểu số BigInt, Kiểu Symbol

Kiểu null: typeof instance === "object".

Object: typeof instance === "object".

Phi dữ liệu Function instance === "function".

---

#### #3 Sự khác biệt giữa null, underfined ?

null : trả về object, và rỗng.

underfined : giá trị không xác định

---

#### #4 Phân biệt var, let, const ?

var: kiểu cũ, trc ES6: khai báo biến kiểu cũ có scope là globally scoped. trừ var nằm trong hàm (scope là function/locally scoped).

##### var dễ gây hoisting: dù khai báo ở đâu biến vấn bị đưa lên đầu hàng.

let: thay thế cho var, scope là block scope.

const: Khai báo hằng.

---

#### #5 Scope là gì? Closure ?

Scope : là phạm vi truy cập: global, local

Closure : Lexical global: hàm trong hàm, hàm con có quyền truy cập đến phạm vi biến của hàm cha.

Khái niệm closure bao đóng. làm cho scope trong không thể tiếp cận được public scope. Chỉ gọi function sẽ không thực hiện gì bởi nó trả về kết quả là tham chiếu tới function.

---

#### #6 Bất đồng bộ là gì ? cơ chế xử lí của JS ?

#### Đồng bộ:

Chương trình sẽ chạy lần lượt theo từng bước và chỉ khi nào thực hiện xong bước 1 mới chuyển sang bước 2, 3, 4…

##### Mặt tốt: Chương trình sẽ chạy đúng thứ tự và có nguyên tắc nên sẽ không mắc các lỗi và tiến trình không cần thiết

##### Mặt xấu: Chương trình chạy lần lượt nên sẽ không sinh ra trạng thái chờ không cần thiết, không tối ưu thời gian, đôi khi gây treo máy.

---

#### Bất đồng bộ:

![async-await](../../images/async-await.png/)

Chương trình có thể nhảy đi bỏ qua một bước nào đó. giả sử công việc 1,2 hoàn toàn độc lập. Nếu công việc thứ 2 xảy ra trước thì sẽ cho ra kết quả trước công việc 1. Không thuộc vào vị trí đặt hàm nào trước.

##### Mặt tốt: Có thể xử lý nhiều công việc cùng một lúc mà không phải chờ đợi, tối ưu được thời gian, hiệu năng và tốc độ

##### Mặt xấu: Nếu chương trình đòi hỏi nhiều quy trình tuần tự thì sẽ gây khó khăn trong quá trình phát triển.

---

#### #7 Event loop là gì, Call stack là gì hoạt động như thế nào ?

Event Loop là cơ chế giúp Javascript có thể thực hiện nhiều thao tác cùng một lúc (concurrent model).

Event Loop có một công việc đơn giản: theo dõi Call Stack và Callback Queue (hàng đợi các hàm callback). Nếu Call Stack đang trống, nó sẽ lấy event đầu tiên từ trong hàng đợi ra và đẩy nó vào trong Call Stack - tức là thực thi nó.

![event loop](../../images/event-loop.png/)

JavaScript là ngôn ngữ lập trình single-threaded.
Call stack là 1 cấu trúc dữ liệu, lưu các lệnh sẽ được thực thi. Vào sau thì ra trước.

[Read more](https://viblo.asia/p/cau-chuyen-xu-ly-bat-dong-bo-trong-javascript-phan-1-YWOZrQAEKQ0)

---

#### #8 So sánh các cách xử lí của JS: callback, promise, async, await…

##### Callback (ES5)

Callback hiểu đơn giản là bạn truyền một hàm B vào hàm A dưới dạng 1 tham số, một lúc nào đó thì hàm A sẽ gọi hàm B để chạy. nhược điểm tạo ra callback hell.

![callback img](../../images/callback.png/)

##### Promise (ES6)

Là "lời hứa" đại diện cho giá trị chưa tồn tại và giá trị đó sẽ được trả về vào một thời gian trong tương lai.

![promise img](../../images/promise.png/)

##### Async / Await (ES7):

Async được dùng để khai báo một hàm bất đồng bộ. Các hàm bất đồng bộ sẽ luôn trả về một giá trị. Việc sử dụng async chỉ đơn giản là ngụ ý rằng một lời hứa sẽ được trả lại và nếu một lời hứa không được trả lại, JavaScript sẽ tự động kết thúc nó.

Await làm cho JavaScript đợi cho đến khi promise trả về kết quả.

#### #9 Các feature trong ES6 là gì ? map, filter, reduce (map, filter, reduce khác gì nhau) ?

---

#### #10 Arrow function ? spread ? set ? destructring ?

Arrow function: là tính năng viết hàm mới của ES6 giúp code ngắn gọn hơn.

Spread Operator : cho phép chuyển đổi một chuỗi thành nhiều argument (trong trường hợp gọi với hàm) hoặc thành nhiều phần tử (cho array).

---

#### #16 String interpolation ?

---

#### #17 Map, Set, Iterator, For-of, Class… ?

---

#### #18 Từ khóa “this”, context ?

"this" để đại diện cho một đối tượng (Object), là chính nó.

---

#### #19 Object, class trong OOP ?

---
