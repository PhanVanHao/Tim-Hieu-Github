# Tim-Hieu-Github
#I.cách thức hoạt động của Github.

 Github hiện đang là server Git lưu trữ source code phổ biến nhất hiện nay .
 Là nơi để lưu code với Repositories

###Cách thức làm việc với GitHub

- Làm việc với GitHub nói riêng hay hệ thống GIT nói chung có 2 workflow chính là local workflow và server workflow.

- Bạn có thể làm mọi chuyện thay đổi source code ở local, sau khi đã thay đổi xong, bạn sẽ commit những thay đổi đó lên server và bản lên server phải là bản hoàn chỉnh một tính năng nào đó, hoặc fix bug xong, test xong hoặc ít nhất bản đó phải chạy được. Không được commit code dở dang, chưa qua test lên repository server sẽ làm ảnh hưởng đến các thành viên khác, ngược lại bạn có thể làm điều đó ở repository local (Bạn cũng có thể tạo một branch ở server cho việc commit code dở dang hay tính năng chưa hoàn thành như từng làm với SVN, nó sẽ chiếm space ở server cũng như làm mất thời gian của bạn vào việc tương tác kết nối với server, vậy tại sao không commit nó lên repository local nhỉ, vừa nhanh thao tác lại không mất space của server.

- Mở rộng: từ repository của github ta có thể theo phương thức của Git tạo bản build cho production site bằng cách push thay đổi lên nó. Khi tương tác với repository server (cập nhật hay thay đổi) GITHUB đòi hỏi mã chứng nhận "Bạn là ai" thông qua so sánh SSH key ở local của bạn và SSH key trên server tương ứng với account mà bạn đã đăng ký với GITHUB trước đó.

#II.Các khái niệm: Add, Remove, Commit, Push, Pull, Fetch, Clone, Fork, Star, Watch.
- **Add** : soạn thảo thêm mới file *đoạn code*
- **Commit** : update bản save hiện tại
- **Push** : đẩy file từ máy trạm lên server(Overwrite)
- **Pull** : kéo file từ server về máy trạm(Overwrite)
- **Fetch**:hủy tất cả thay đổi và commit cục bộ, lấy về (fetch) lịch sử gần đây nhất từ máy chủ và trỏ nhánh master cục bộ vào nó
- **Clone**: sao chép một repository
- **Fork** : Lấy repo của người khác về trang cá nhân
- **Star** : Gắn sao , tiện xem lại
- **Watch** : Theo dõi Repo, nhận thông báo

#III.
##1.Seting up git 
Download tại địa chỉ: https://windows.github.com/
![Anh down load](http://sv1.upsieutoc.com/2016/12/09/anh.png)

Cài đặt bình thường, yêu cầu phải có .NET 4.5

Giao diện của chương trình:
![giao dien](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09200648.png)

**Thêm tài khoản Github:**

- Click vào tool and options (hình bánh răng cạnh biểu tượng Sync) chọn options, Add account. Khai báo username và password trên github.

- Tại mục Configure git thêm Tên và email của mình

![ACC](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09200829.png)

#2.Thao tác với Repo
2.1. Tạo một repo mới

Tạo repo trên github.com 
![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09201045.png)
![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09201128.png)

Tạo repo bằng phần mềm Github

Click vào dấu cộng, chọn tab Create, đặt tên và chọn đường dẫn cho repo mới

![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09201239.png)

Tuy nhiên repo mới sinh ra mới chỉ có ở máy trạm, tại mục **Other**. Chọn chuột phải vào repo đó và chọn **Open in Explorer** để sửa nội dung của repo này.
![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09201503.png)

Sau khi chỉnh sửa xong, để đẩy repo đó lên github.com ta click vào **Publish this repository** và thực hiện như hình sau. Chú ý cần chọn **Organization** đặt repo này.
![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09201657.png)

2.2. Clone

Click vào dấu cộng, chọn tab Clone, lựa chọn tổ chức mong muốn và chọn repo cần clone

![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09202103.png)
![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09201859.png)

Để chỉnh sửa nội dung của repo này ta chọn chuột phải vào nó và chọn Open in Explorer
Lúc đó chương trình Windows Explorer sẽ mở ra thư mục chứa repo của github, bạn có thể chỉnh sửa các file trong này, tạo xóa thư mục,... một cách bình thường.

2.3. Add, commit, push, pull

Trở lại với chương trình Github ta sẽ thấy dòng **x changes** tại repo ta vừa sửa. Bạn hãy điền vào đó **comment** và ấn **commit to master**

![](http://sv1.upsieutoc.com/2016/12/09/Clipboardimage2016-12-09202319.png)







