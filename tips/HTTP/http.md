<div align="center">
<h3>HTTP/ HTTPS</h3>
</div>

**Begin:**

- HTTP: là từ viết tắt của HyperText Transfer Protocol, dạng giao thức truyền tải chuẩn của mạng Internet
- HTTPS: là http nhưng thêm security là bảo mật.
- HTTP: có 2 dạng là HTTP Request và HTTP Response. Request dùng để gửi yêu cầu từ phía người dùng (client) lên phía server. Ngược lại thì Respone lại được gửi từ phía server cho client.

**Status code:**
> Là các mã số mà server sẽ trả về cho phía client để định nghĩa tiếp các action tiếp theo.
> Chắc bạn nhìn thấy cãi trang 404 ở đâu đố rồi chứ. 404 là một HTTP status code.


Có 5 loại status code hiện tại đang được sử dụng rộng rãi:
- [1xx - Infomation: Khi nhận những status code này thì có thể hiểu là request đã được server tiếp nhậrn và đang trong quá trình xử lý.](#1xx-Infomation)
- [2xx - Success: Request đã được server tiếp nhận và xử lý thành công.](#2xx-success)
- [3xx - Redirection: Client cần có thêm action để hoàn thành request.](#3xx-Redirection)
- [4xx - Client Error: Client request lên cú pháp không chính xác hoặc bị lỗi.](#4xx-client-errorr)
- [5xx - Server Error: Server thất bại với việc thực hiện một request của client.](#5xx-server-error)


### Chi tiết về HTTP Status code:

#### 1xx Infomation:
- 100 Countinue
- 101 Switching Protocols

#### 2xx Success:
- 200 OK
- 201 Created
- 202 Accepted
- 204 No-Content

#### 3xx Redirection:
- 304 Not Modified

#### 4xx Client Errorr:
- 400 Bad Request
- 401 Unauthorized
- 403 Forbiden
- 404 Not Found
- 405 Method Not Allowed

#### 5xx Server Error:
- 500 Internal Server Error
- 502 Bad Gateway
- 504 Gateway timeout

**Note**: Đây ***không phải*** là toàn bộ status code mà mình chỉ đưa ra một só cái hay gặp thôi.