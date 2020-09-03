<div align="center">
<h1>
	Comment trong code
</h1>
	<img src="https://s3-ap-southeast-1.amazonaws.com/kipalog.com/ls5miadipf_comment-code-4.jpg" alt="comment"/  >
</div>

<hr />

## Tại sao chúng ta cần phải comment code?
> Chúng ta luôn tự hỏi, khi code một function, một class, một struct, một file,... thì có cần phải comment hay không trong khi từng cái tên của function đã mô mục đích sử dụng function đó. Nhưng nếu như bạn để ý thì không hẳn như vậy. Chúng ta có nhiều function nhưng với mỗi function có nhiều param( tham số truyền vào) khác nhau, nếu không comment đoạn code lại thì làm sao người khác có thể đọc và hiểu được. Nếu như bạn để ý các blog khi viết code cũng thường comment( kiểu inline) để cho mọi người dễ hiểu. 

> Ok, chưa dừng lại ở việc comment function, chúng ta còn có cả comment một file( do ai tạo ra, ngày tạo ra, ngày update), comment dạng TODO: ghi những yêu cầu, công việc của function. Lý do bạn lên viết comment code đó là một số tool có thể tự tạo tài liệu mô tả khi bạn comment.

<hr />

## Khi nào không nên comment code?
> Bên trên là một đống lý do để comment code, nhưng điều đó không đồng nghĩa với việc bạn comment một cách bừa bãi. Code một dòng lại comment lại như kiểu này: 
```
// The class definition for Account
public class Account {
    //Constructor
    Account();

    // Set the profit member to a new value
    public void SetProfit(double profit);

    // Return the profit from this Account
    public double GetProfit();
};
```
> Bạn thấy rồi đấy, comment như này là thừa thãi, trừ khi bạn đang cố giải thích tường tận cho người ra rằng đoạn code đó đang làm gì? (Tất nhiên chỉ giải thích cho người mới thôi, còn trong project thực tế, gần như không sử dụng comment thế này).

> Khi bạn maintain một dự án, một vài function không còn phù hợp nữa, bạn muốn xóa nó đi thì cũng đừng quên xóa luôn cả comment của nó nhé. Lúc đó comment chẳng còn ý nghĩa gì cả vì làm gì còn function cần nó diễn tả đâu.
<hr />

## Comment chuẩn bài là thế nào?
> Giờ đến tiết mục quan trọng nhất: Khi nào cần comment? Comment thế nào cho chuẩn bài?

> Mục đích comment là cho người khác đọc vào code của bạn dễ hiểu hoặc chính bạn khi đọc lại code cũng có thể hiểu được(đừng để tự mình lúc đó chửi mình).

> Khi nào chúng ta cần comment:
 1. Khi cần nói rõ ý định sẽ làm gì:
	 - Bạn nên comment lại toàn bộ mục đích khi sử dụng hàm, các tham số truyền vào, kết quả đầu ra sẽ như thế nào.
 2. Comment nhưng đoạn code phức tạp, nhiều vòng lặp nối tiếp nhau, nhiều if-else liền nhau:
	 - Khi gặp những trường hợp thế này, hãy cố gắng comment trước các vòng lặp để làm tường minh cái ý định của mà bạn sẽ làm với đống code đó.


> Chuẩn comment xin phép được bắt đầu:


 **a. Comment in-line:**
```
// kiểm tra khi đưa một id vào, id đó có tồn tại trong database không. Nếu đúng trả về true, sai trả về false
```

**b. Comment Header file ( lưu ý là comment trong file Main class)**
```
/*
 * 
 * Created on Tue Feb 18 2020
 *
 * Copyright (c) 2020 - Your Company
 */
```

**c. Class Header comment**
```
/**
 * (Write a succinct description of this class here. You should avoid
 * wordiness and redundancy. If necessary, additional paragraphs should
 * be preceded by <p>, the html tag for a new paragraph.)
 *
 * <p>Bugs: (a list of bugs and other problems)
 *
 * @author tjjone98
 */
```
**d. Method Header comment**
```
/**
 * (Write a succinct description of this method here.  If necessary,
 * additional paragraphs should be preceded by <p>, the html tag for
 * a new paragraph.)
 *
 * @param (parameter name) (Describe the first parameter here)
 * @param (parameter name) (Do the same for each additional parameter)
 * @return (description of the return value)
 */
```
**e. Comment trong styles css**

Cá nhân mình thì thích kiểu comment group:
```
/** @group footer */
#footer {
 color: white;
}
```