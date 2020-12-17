---
title: "Reactjs"
date: 2020-12-15T03:18:36+07:00
---

#### #1 Read DOM, Virtual DOM ?

DOM (Document Object Model) : là mô hình đối tượng tài liệu HTML. thao tác với DOM phải đi từ root ra.

VDOM (Virtual Dom) : Từ Dom thật, React sao chép bản thiết kế Dom này, sau đó, mỗi thao tác chỉnh Dom sẽ không thông qua method dành cho Dom, mà thông qua API của React.

Khi tất cả các thay đổi đã được update trên DOM ảo, React sẽ kiểm tra xem thay đổi cụ thể nào cần được áp dụng vào DOM gốc (bởi thuật toán so sánh diff của React), và áp dụng thay đổi này vào chính xác chỗ cần thay đổi.

---

#2 LifeCycle ?

[Read more](https://viblo.asia/p/lifecycle-component-trong-reactjs-gGJ59jzxKX2)

![alt text](../../resources/gen/images/lifecycle.png)

---

#3 Data binding là gì ?

---

#4 GET, POST là gì, khác nhau như thế nào? Giả sử muốn upload một file thì làm như thế nào ?

---

#5 Hook ? UseEffect ?

---

#### #6 Prop ? State ?

Props: Dữ liệu đầu vào, truyền từ trên xuống dưới. Thằng con ko thể chỉnh sửa thằng cha.

State: Thuộc sở hữu của component. Được khởi tạo và có thể cập nhất bất cứ khi nào cần thiết. Thường state của component cha thường là props của components con.

---

#7 Graph ?

---

#8 Phân biệt stateless vs statefull ?

---

#9 Class components vs Functional components ?

---

#10 Stateful component vs Stateless component ?

---

#11 Webpack là gì ?

---
