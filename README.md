# Cplusplus-Base

## Structs
https://cpp.daynhauhoc.com/9/1-structs/
* Như các bạn thấy, việc quản lý chương trình trở nên phức tạp so với những người mới học lập trình. Do đó, việc tự định nghĩa một kiểu dữ liệu mới phù hợp cho đặc thù của chương trình của mỗi người là điều cần thiết. Rất may mắn, ngôn ngữ C++ hổ trợ chúng ta tự định nghĩa kiểu dữ liệu mới từ những kiểu dữ liệu built-in. Kiểu dữ liệu mới mà chúng ta sẽ định nghĩa được tạo thành từ một hoặc một nhóm kiểu dữ liệu xây dựng sẵn để tạo ra một tập hợp các biến thuộc cùng nhóm, những biến cùng nhóm này dùng để lưu trữ các dữ liệu có liên quan với nhau trong kiểu dữ liệu mới. Chúng ta gọi kiểu dữ liệu tập hợp này là struct.  

* Một struct (viết tắt của structure) cho phép chúng ta nhóm nhiều biến của nhiều kiểu dữ liệu khác nhau để lưu trữ một tập hợp các dữ liệu cần thiết cho việc mô tả một đơn vị nào đó.  

* Để khai báo một cấu trúc mới (kiểu dữ liệu mới), chúng ta sử dụng từ khóa struct. Mặc dù một struct là một kiểu dữ liệu do lập trình viên tự định nghĩa, nó cũng cần được khai báo theo một cú pháp nhất định để compiler có thể hiểu được. Dưới đây là cú pháp để tạo ra một struct mới:

	```C++
	struct <name_of_new_type>
	{
		<variables>;
	};
	```

	Trong đó:  
	**struct** là từ khóa mà ngôn ngữ C++ cung cấp.  
	**name_of_new_type** sẽ là tên của kiểu dữ liệu mới. Sau khi khai báo xong một struct, chúng ta có thể dùng tên struct để khai báo biến như những kiểu dữ liệu thông thường.  
	variables là danh sách các biến dùng để lưu trữ dữ liệu phù hợp với yêu cầu lưu trữ dữ liệu của một đơn vị nào đó.  

## inline
* Khi được nạp vào ram, mỗi hàm sẽ có địa chỉ nhất định, khi gọi thì cpu sẽ jump tới địa chỉ đó.
Viết inline thì compiler sẽ chèn luôn code của hàm đó vào, thay vì chèn địa chỉ, cpu chỉ chạy một mạch mà thôi, vậy nên sẽ nhanh hơn. Chỉ nên dùng cho getter và setter vì nó nhẹ mà hay được gọi

* Inline về cơ bản nó sẽ không tạo ra lời gọi hàm mà chèn trực tiếp mã vào nơi hàm được gọi > tăng size (cụ thể là của file thực thi).
Giống như việc bạn học bài thi học kì, thầy cho đề cương gồm nhiều câu hỏi tự luận. Bạn thích gom các câu trả lời vào chung 1 tờ giấy A4 cho dễ học, đỡ mất thời gian học từng bài, hay chỉ cần đánh dấu trong vở những phần cần học.  
  Sử dụng inline cũng vậy.

* Hàm được khai báo “inline” không có nghĩa là compiler sẽ bắt buôc phải inline nó, mà tùy thuộc vào hàm mà compiler có inline hay không.
Không phải lúc nào cũng dùng hàm “inline” bởi vì khi hàm được inline quá dài và sử dụng nhiều lần trong source code, nó sẽ expand ra và làm tăng size của chương trình lên rất nhiều. Vì thế, thường ta sẽ inline những hàm có body ngắn thôi.

## Get/Set
* Các thành phần bên trong cần giới hạn truy cập, vì thế sinh ra việc sử dụng hàm.  
   Quy luật bất biến của module hoá, S trong SOLID , mỗi hàm chỉ làm và thực hiện một việc duy nhất. Vậy thì hàm SET thì chỉ có SET giá trị vào, còn GET thì chỉ GET giá trị ra. Không thể nhét cả GET/SET vô trong một hàm.  
   Trong lập trình, hàm viết càng nhỏ càng tốt, càng ít logic càng tốt. Vẫn theo quy tắc cũ 80 cột / 25 hàng tối đa cho một hàm.  
   Với một số ngôn ngữ lập trình bậc cao như C#, thì việc GET/SET được quy về một cái gọi là ĐẶC TÍNH (hay tiếng Anh là PROPERTY), chỉ cần khai báo 1 lần trong code thôi. Nhưng về bản chất code sinh ra trước khi biên dịch thì sẽ tách ra thành 2 hàm, một GET, một SET cả thôi.  

* Đặc trưng oop  
   lấy hoặc thay đổi gía trị của biến private nội bộ lớp thông qua phương thức get, set

## Xử lý ngoại lệ trong ngôn ngữ C++
https://daynhauhoc.com/t/xu-ly-ngoai-le-trong-ngon-ngu-c/74926  

## Namespace
https://www.stdio.vn/articles/tu-khoa-namespace-59  
Namespace là một cơ chế trong C++, cho phép ta nhóm các thực thể (class, object, function…) có liên quan thành từng nhóm khác nhau theo tên, mà theo đó tên của mọi thực thể trong mỗi namespace đều được gắn thêm tên của namespace đó như tiền tố.  

## Truy cập thuộc tính và method trong class hoặc struct
* Thuộc tính, method thông thường    
	Toán tử "."  
* Thuộc tính, method là con trỏ  
	Toán tử "->"  

## Template
https://cowboycoder.tech/article/c-co-ban-phan-27-template-thu-vien-template-chuan-cua-c  

## Dau & trong C++
https://daynhauhoc.com/t/hoi-ve-dau-trong-c/1121  

## Vector3f
https://stackoverflow.com/questions/57810925/convenient-vector3f-class  
