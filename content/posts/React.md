---
title: "Reactjs"
date: 2020-12-15T03:18:36+07:00
---

#### #1 Read DOM, Virtual DOM ?

DOM (Document Object Model) : là mô hình đối tượng tài liệu HTML. thao tác với DOM phải đi từ root ra.

VDOM (Virtual Dom) : Từ Dom thật, React sao chép bản thiết kế Dom này, sau đó, mỗi thao tác chỉnh Dom sẽ không thông qua method dành cho Dom, mà thông qua API của React.

Khi tất cả các thay đổi đã được update trên DOM ảo, React sẽ kiểm tra xem thay đổi cụ thể nào cần được áp dụng vào DOM gốc (bởi thuật toán so sánh diff của React), và áp dụng thay đổi này vào chính xác chỗ cần thay đổi.

---

#### #2 LifeCycle ?

[Read more](https://viblo.asia/p/lifecycle-component-trong-reactjs-gGJ59jzxKX2)

![lifecycle img](https://images.viblo.asia/c3c37d71-9a8f-4250-b7a3-d01cb1cc525e.png)

---

#3 Data binding là gì ?

---

#4 GET, POST là gì, khác nhau như thế nào? Giả sử muốn upload một file thì làm như thế nào ?

---

#### #5 Hook ? UseEffect ?

Hooks : cho phép "kết nối" React state và lifecycle vào các components sử dụng hàm mà không cần dùng ES6 class.

useEffect để tiếp cận vào các lifecycles, bằng với componentDidMount, componentDidUpdate , componentWillUnmount và chỉ chạy sau khi render.

![useEffect](../../images/useEffect.png/)

[counter] = bằng với= prevState.counter !== this.state.counter

![useEffect](../../images/didUpdate.png/)

[Read more hooks](https://ehkoo.com/bai-viet/react-hooks-la-gi)

---

#### #6 Prop ? State ?

Props: Dữ liệu đầu vào, truyền từ trên xuống dưới. Thằng con ko thể chỉnh sửa thằng cha.

State: Thuộc sở hữu của component. Được khởi tạo và có thể cập nhất bất cứ khi nào cần thiết. Thường state của component cha thường là props của components con.

---

#7 Graph ?

---

#### #8 Phân biệt stateless vs statefull ? Stateful component vs Stateless component ?

stateful component: luôn là class component. Cập nhật state bằng hàm setState();

stateless component: có thể dùng hàm hoặc lớp để tạo (nếu ko cần sử dụng lifecycle thì nên dùng functional components

---

#### #9 Class components vs Functional components ?

Class components: có thể có state. Có thể định nghĩa hàm khởi tạo.

Functional components: chỉ là hàm javascript nhận các tham số truyền vào (props). Muốn xử lý state trong này phải dùng hooks.

---

#10 Webpack là gì ?

---

#11

---
