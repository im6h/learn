> Có một câu nói: Học Regex đi, rồi đời bạn sẽ bớt khổ đau.

#### Start:

Chúng ta sẽ bắt đầu với những thứ đơn giản nhất của Regex:

- [xyz]: đơn giản nhất là tìm và so sánh tất cả ký tự nằm trong dấu ngoặc vuông và trùng khớp với 1 ký tự trong dấu ngoặc vuông. Như ở trên sẽ trùng khớp x hoặc y hoặc z.
- [a-z]: so sánh trùng khớp với một ký tự nằm trong khoảng chỉ định, ví dụ sẽ trùng với kí tự a-z nằm trong chuỗi cần test.
- [0-9]: so sánh trùng khớp với một ký tự nằm trong khoảng chỉ định, trùng với kí tự từ 0 đến 9 nằm trong chuỗi cần test.
- [^xyz]: nằm trong ngoặc vuông là phủ định của [xyz]. Tương tự thế [^a-z] là phủ định của [a-z].
- ^a: trùng khớp với chữ a đứng ở đầu trong chuỗi.
- ^\w+:trùng khớp từ đầu tiên của chuỗi.
- c$: trùng khớp chữ c ở cuối chuỗi.
- \w+$:trùng khớp từ cuối cùng của chuỗi.
- +: trùng khớp với 1 hoặc nhiều lần ký tự đứng trước nó. Ví dụ \d+ sẽ chỉ trùng khớp với phần của có từ 1 chữ số trở lên
-  *  :Trùng khớp với 0 hoặc nhiều lần ký tự đứng trước nó. Ví dụ \d* sẽ trùng với chuỗi có chứa 1 chữ số hoặc k có chữ số nào cũng đc.