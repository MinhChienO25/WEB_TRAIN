**TASK 0**
1. The HTTP Protocol(HyperText Transfer Protocol)
* Là giao thức chuẩn được sử dụng để truyền tải phương tiện kỹ thuật số qua Internet và tải các trang web bằng siêu liên kết.
* HTTP là một giao thức ứng dụng của bộ giao thức TCP/IP là phương thức được sử dụng để truy xuất dữ liệu từ server ở một tài nguyên rõ ràng đã được chỉ định.
2. HTTP Requests
* Là một thông điệp mà máy khách gửi đến máy chủ để yêu cầu một tài nguyên hoặc một hành động. Các tài nguyên này có thể là bất cứ thứ gì, từ các trang HTML và hình ảnh đến các tệp, video hoặc thậm chí là các bản ghi cơ sở dữ liệu.
* Mỗi HTTP Request đều tuân theo một định dạng chuẩn bao gồm:
   - Request Line:là dòng máy khách gửi đi để bắt đầu hành động trên máy chủ, bao gồm 3 thành phần chính là:method, request-target,protocol.
   - Header:cho phép truyền thông tin giữa máy chủ và máy khách
   - Body:là phần chứa thông tin gửi đến máy chủ
![HTPP REQUEST](https://hackmd.io/_uploads/SyJh8icKfg.png)
3. HTTP Responses
* Là các thông báo HTTP mà máy chủ gửi lại để đáp lại yêu cầu.Mục đích của  là cung cấp cho máy khách tài nguyên yêu cầu, hoặc thông báo cho máy khách rằng yêu cầu đã được thực hiện; hoặc thông báo cho máy khách rằng đã xảy ra lỗi trong quá trình xử lý yêu cầu.
* Một HTTP Responses bao gồm:
   - Status-line:Cho biết yêu cầu đã thành công, thất bại hay cần thực hiện thêm thao tác, bao gồm 3 phần:HTTP Version, Status-code, Reason-phrase
   - Response headers: mô tả các đặc điểm của phần thân thông báo. HTTP Responses headers được cấu trúc dưới dạng các cặp key/value.
   - Response Body: nội dung phản hồi lại máy khách khi yêu cầu thành công, có thể chứa nhiều định dạng như html, images,...
 ![HTTP RESPONSE](https://hackmd.io/_uploads/B10RlFsKfl.png)
4. HTTP Methods
* GET:  là phương thức được sử dụng để truy xuất dữ liệu từ server ở một tài nguyên rõ ràng đã được chỉ định. Ta dùng GET để lấy danh sách tài nguyên, tìm kiếm và lọc dữ liệu, hoặc bất kì thao tác chỉ đọc nào.
* HEAD: Giống GET nhưng chỉ trả về headers, không trả về body. Ta dùng HEAD để kiểm tra resource có tồn tại không, file có thay đổi không, link có còn hoạt động không,...
* POST: Tạo mới tài nguyên hoặc gửi dữ liệu để xử lý trên server. Ta dùng POST khi muốn tạo mới tài nguyên, upload file hoặc xử lý dữ liệu phức tạp 
* PUT: Cập nhật trạng thái tài nguyên hoặc ghi đè nó. Ta dùng PUT khi muốn cập nhật toàn bộ thông tin user hoặc thay thế hoàn toàn một tài nguyên.
* DELETE: Xóa tài nguyên trên sever. Ta dùng DELETE khi muốn xóa user, sản phẩm, bài viết, comment hoặc bất kì thao tác xóa tài nguyên nào
* CONNECT: thiết lập một đường hầm TCP/IP đến máy chủ.Nó được sử dụng để bảo mật giao tiếp hai chiều thông qua một hoặc nhiều máy chủ proxy HTTP với SSL/TLS. 
* OPTIONS: sử dụng để mô tả các tùy chọn giao tiếp cho tài nguyên đích. Ta dùng OPTIONS để kiểm tra API hỗ trợ những phương thức nào để có thể sử dụng chúng.
* TRACE: thực hiện kiểm tra vòng lặp thông báo dọc theo đường dẫn đến tài nguyên đích.Bằng cách đó, máy khách có thể thấy liệu có bất kỳ thay đổi hoặc bổ sung nào đã được thực hiện bởi các bên trung gian hay không.
* PATCH: Cập nhật một phần tài nguyên.Ví dụ: cập nhật email, status hoặc bất kì thao tác cập nhật một phần nào.
5. URLs (Uniform Resource Locator)
* Là địa chỉ định danh của một tài nguyên trên INTERNET. Khi người dùng nhập URL vào trình duyệt, trình duyệt sẽ gửi yêu cầu tới máy chủ tương ứng để truy xuất đúng dữ liệu cần hiển thị.
* Các thành phần của URL có thể bao gồm:
  - Giao thức hoặc lược đồ: để truy cập tài nguyên trên Internet. Các giao thức có thể bao gồm: http,https,ftps,...
  - Tên máy chủ hoặc tên miền: mã định danh duy nhất đại diện cho một trang web.
  - Tên miền phụ: đứng trước tên miền chính
  - Tên cổng: luôn đứng sau dấu hai chấm và thường không hiển thị trong URl.
  - Đường dẫn: đề cập đến một tệp hoặc vị trí trên máy chủ web.
  - Truy vấn: Thường xuất hiện trong URL của các trang động, truy vấn bao gồm dấu chấm hỏi, theo sau là các tham số hoặc chuỗi truy vấn.
  - Tham số: là các phần thông trong chuỗi truy vấn của URl. Nhiều tham số có thể được phân tách bằng dấu và (&).
  - Đoạn trích: là một tham chiếu nội bộ đến một phần trong trang web. Nó xuất hiện ở cuối URL và bắt đầu bằng dấu thăng (#).
  
  ![URL](https://hackmd.io/_uploads/BkesvTnFMe.png)

6. HTTP Headers
* HTTP Headers là các metadata (dữ liệu về dữ liệu) được gửi kèm với HTTP request và response. Headers cung cấp thông tin bổ sung về request/response hoặc về dữ liệu được gửi trong message body
* Request Headers:
  - Accept:thông báo cho server loại dữ liệu nào có thể được trả về.
  - Accept-Encoding: Thông báo cho máy chủ biết loại mã hóa nội dung nào mà máy khách sẵn sàng chấp nhận, giúp giảm dung lượng truyền tải và tăng hiệu suất tải trang.
  - Authorization: xác thực người dùng với server thường chứa mã token hoặc thông tin đăng nhập theo chuẩn HTTP Auth.
  - Cookie: chứa các cặp key/value của cookie mà client lưu trước đó, server sử dụng để nhận diện phiên làm việc hoặc trạng thái người dùng.
  - Host: xác định tên miền và số cổng của server mà client đang gửi yêu cầu tới.
  - If-Modifield-Since: cho phép thực hiện các yêu cầu có điều kiện bằng cách yêu cầu máy chủ chỉ trả về tài nguyên nếu nó đã được sửa đổi sau một ngày cụ thể.
  - If-none-match:yêu cầu sever chỉ trả về tài nguyên nếu etag không khớp với bất kỳ giá trị nào client gửi, dùng kiểm tra tài nguyên mới.
  - Origin: cho biết nguồn gốc (lược đồ, tên máy chủ và cổng) đã khởi tạo yêu cầu.
  - Referer: Chỉ định URL từ yêu cầu đã được khởi tạo gần đây. Điều này giúp máy chủ hiểu được lưu lượng truy cập đến từ đâu.
  - User-Agent: xác định trình duyệt web hoặc ứng dụng khách thực hiện yêu cầu, cho phép máy chủ điều chỉnh phản hồi phù hợp với khả năng của máy khách. 
* Response Headers:
  - `Access-Control-Allow-Origin`: Đây là tiêu đề phản hồi mà máy chủ gửi lại cho trình duyệt để thông báo: “Nguồn gốc này được phép đọc phản hồi của tôi.
  - `Cache-Control`: kiểm soát hành vi lưu trữ tạm thời trong trình duyệt của máy khách hoặc các bộ nhớ đệm trung gian. Nó xác định cách phản hồi có thể được lưu vào bộ nhớ đệm, khi nào nó hết hạn và cách nó nên được xác thực lại. Bao gồm các giá trị như:
     - Max-age:khoảng thời gian cần thiết để bản sao được lưu trong bộ nhớ cache của một tài nguyên hết hạn) 
     - No-cache:trình duyệt có thể lưu trữ phản hồi, nhưng trước tiên phải gửi yêu cầu xác thực đến  máy chủ gốc.
     - No-store:trình duyệt không được phép lưu trữ phản hồi vào bộ nhớ cache và phải tải phản hồi từ máy chủ mỗi khi được yêu cầu.
     - Public:cho biết rằng một tài nguyên có thể được lưu vào bộ nhớ đệm bởi bất kỳ bộ nhớ đệm nào.
     - Private: cho biết tài nguyên đó chỉ dành riêng cho người dùng — nó vẫn có thể được lưu vào bộ nhớ đệm, nhưng chỉ trên thiết bị của người dùng
  - Etag: cung cấp một mã định danh duy nhất cho một phiên bản cụ thể của tài nguyên.Client có thể gửi mã định danh này trong tiêu đề `If-None-Match` để thông báo cho máy chủ biết phiên bản tài nguyên nào đang được trình duyệt lưu trong bộ nhớ đệm.
  - Expires: chỉ định ngày/giờ cố định cho việc hết hạn của tài nguyên được lưu trong bộ nhớ cache.
  - Locations: Sử dụng trong quá trình chuyển hướng để chỉ định đích đến của quá trình chuyển hướng.
  - Pragma: dùng để kiểm soát bộ nhớ đệm,sử dụng để đảm bảo khả năng tương thích ngược với HTTP/1.0.
  - Sever: mô tả phần mềm được máy chủ gốc sử dụng để xử lý yêu cầu và tạo ra phản hồi
  - Set-Cookie: cung cấp các cookie cho trình duyệt, và trình duyệt sẽ gửi lại các cookie đó cho máy chủ trong các yêu cầu tiếp theo.
  - WWW-Authenticate: đóng vai trò hỗ trợ cho nhiều cơ chế xác thực khác nhau, rất quan trọng để kiểm soát quyền truy cập vào các trang và các tài nguyên khác dựa trên việc sử dụng mã trạng thái 401.
  - X-Frame-Options: được sử dụng để chỉ ra liệu trình duyệt có được phép hiển thị tài liệu trong thẻ `frame`, `iframe`, `embed` hoặc `object` hay không.
7. Cookies
* Cho phép máy chủ gửi dữ liệu đến máy khách; máy khách sẽ lưu trữ và gửi lại dữ liệu này cho máy chủ. Một cookie thông thường bao gồm một cặp key/value nhưng chúng cũng có thể bao gồm bất kỳ chuỗi ký tự nào không chứa dấu cách.Ngoài giá trị thực tế của Cookie, `Set-Cookie` có thể bao gồm bất kì thuộc tính nào dưới đây, giúp kiểm soát việc trình duyệt xử lý cookie:
  - `Expires`: thiết lập thời hạn mà cookies còn hiệu lực, nếu không được thiết lập thì cookies chỉ được dùng trong thời gian làm việc của trình duyệt.
  - `domain`: chỉ định tên miền mà cookie được nhận
  - `path`: chỉ định đường dẫn URL mà cookie đó hợp lệ.
  - `secure`: chỉ được gửi trong HTTP Request.
  - `HttpOnly`: cookie sẽ không thể được truy cập trực tiếp thông qua JavaScript phía Clients.
8. Status Codes
* Là một số nguyên có ba kí tự. Kí tự đầu tiên định nghĩa loại Response và hai kí tự cuối không có trị phân loại nào. Status Code chia làm 5 loại:
  - 1xx: Information: tức là request đã được server tiếp nhận và quá trình đang được tiếp tục. 
  - 2xx: Success: tức là request đã được server tiếp nhận, hiểu và xử lý thành công.
  - 3xx: Redirection: cho biết client cần có thêm hành động để hoàn thành request.
  - 4xx: Client Error: Request chứa một lỗi nào đó.
  - 5xx: Server Error: Máy chủ gặp lỗi khi thực hiện yêu cầu
* Có rất nhiều Status code, dưới đây là một số mã có khả năng gặp phải khi tấn công web:
  - `100 Continue`: cho biết rằng các tiêu đề yêu cầu đã được nhận và máy khách nên tiếp tục gửi phần thân.
  - `200 Ok`: yêu cầu được tiếp nhận và xử lý thành công
  - `201 Created`: Yêu cầu đã được xử lý và kết quả tạo ra một resource mới.
  - `301 Moved Permanetly`: Request hiện tại và các request sau được yêu cầu di chuyển tới một URI mới.
  - `302 Found`: thông báo cho trình duyệt rằng trang web đã chuyển hướng đến một địa chỉ khác.
  - `304 Not Modifield`: cho biết rằng tài nguyên yêu cầu chưa thay đổi kể từ khi nó được lần cuối lưu trữ trong cache của trình duyệt
  - `400 Bad Request`: thông báo cho người dùng biết rằng hiện máy chủ web không thể xử lý truy vấn do sự cố nào đó.
  - `401 Unauthorized`:  báo hiệu rằng người dùng chưa được ủy quyền để truy cập tài nguyên trên website hoặc máy chủ
  - `403 Forbidden`: cho biết không ai được phép truy cập vào tài nguyên được yêu cầu, bất kể đã xác thực hay chưa.
  - `404 Not Found`: cho biết tài nguyên được yêu cầu không tồn tại
  - `405 Method Not Allowed`: cho biết phương thức được sử dụng trong yêu cầu không được hỗ trợ cho URL được chỉ định
  - `413 Request Entity Too Large `: xảy ra khi bạn cố upload một file quá lớn tới server
  - `414 Request URI Too Long`: cho biết URL được sử dụng trong yêu cầu quá lớn so với khả năng xử lý của máy chủ.
  - `500 Internal Server Error`: xuất hiện khi máy chủ của website bạn đang truy cập bị lỗi, gặp sự cố, không thể hiển thị nội dung hay thông tin gì.
  - `503 Service Unavailable`:  thông báo cho người dùng rằng máy chủ không thể xử lý yêu cầu của của bạn.
9. HTTPS
- Là giao thức HTTP truyền thống được bổ sung các phương thức bảo mật để tăng độ an toàn cho website.
- HTTPS sử dụng các chứng chỉ SSL (Secure Sockets Layer) giúp mã hóa dữ liệu truyền tải nhằm gia cố bảo mật giữa Web sever đến các trình duyệt web.
- HTTPS có thể mã hóa thông tin,đảm bảo tính toàn vẹn và tính riêng tư
10. HTTP Proxies
* Là một máy chủ trung gian hoạt động giữa thiết bị khách và máy chủ web. Một quy trình của proxies đơn giản gồm ba bước: bạn gửi yêu cầu đến máy chủ proxies, máy chủ proxies gửi yêu cầu đến trang web, và trang web phản hồi lại thông qua máy chủ proxies. Không phải tất cả các máy chủ proxy đều giống nhau. Chúng được thiết kế cho các mục đích khác nhau.
  | Loại Proxies                 | Chức năng chính | 
  | --------                     | --------                                        |
  | Forward Proxy                | Thay mặt người dùng yêu cầu dữ liệu từ Internet |
  | Reverse Proxy                | Thay mặt máy chủ xử lý các yêu cầu từ máy khách |
  |Transparent Proxy             |  chặn lưu lượng truy cập của bạn và chuyển tiếp nó mà không che giấu địa chỉ IP thực của bạn khỏi trang web đích|
  |Anonymous Proxy               |Ẩn địa chỉ IP của người dùng và tự nhận mình là máy chủ proxy|
  | Elite (High-Anonymity) Proxy |Ẩn địa chỉ IP của người dùng và không tự nhận mình là máy chủ proxy|
11. HTTP Authentication
* Là một cơ chế bảo mật giúp xác minh danh tính người dùng khi họ truy cập vào các tài nguyên web bằng nhiều phương thức khác nhau, bao gồm:
  - Basic: yêu cầu người dùng cung cấp tên đăng nhập và mật khẩu cho mỗi yêu cầu và được mã hóa bằng Base64 và gửi trong tiêu đề Authorization của HTTP request.
  - Digest: máy chủ gửi một giá trị nonce (số lần sử dụng) và yêu cầu client sử dụng nó để tạo một chuỗi mã hóa. Phương thức này sử dụng thuật toán MD5 để mã hóa thông tin đăng nhập.
  - Bearer: Client gửi yêu cầu đăng nhập để nhận token, sau đó gửi token này trong mỗi request tiếp theo để xác thực.
  - NTLM: Đây là cơ chế challenge-response và sử dụng một phiên bản giao thức NTLM của Windows.

