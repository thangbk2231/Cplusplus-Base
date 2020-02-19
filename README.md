# Cplusplus-Base

## Structs
Như các bạn thấy, việc quản lý chương trình trở nên phức tạp so với những người mới học lập trình. Do đó, việc tự định nghĩa một kiểu dữ liệu mới phù hợp cho đặc thù của chương trình của mỗi người là điều cần thiết. Rất may mắn, ngôn ngữ C++ hổ trợ chúng ta tự định nghĩa kiểu dữ liệu mới từ những kiểu dữ liệu built-in. Kiểu dữ liệu mới mà chúng ta sẽ định nghĩa được tạo thành từ một hoặc một nhóm kiểu dữ liệu xây dựng sẵn để tạo ra một tập hợp các biến thuộc cùng nhóm, những biến cùng nhóm này dùng để lưu trữ các dữ liệu có liên quan với nhau trong kiểu dữ liệu mới. Chúng ta gọi kiểu dữ liệu tập hợp này là struct.  

Một struct (viết tắt của structure) cho phép chúng ta nhóm nhiều biến của nhiều kiểu dữ liệu khác nhau để lưu trữ một tập hợp các dữ liệu cần thiết cho việc mô tả một đơn vị nào đó.  

Để khai báo một cấu trúc mới (kiểu dữ liệu mới), chúng ta sử dụng từ khóa struct. Mặc dù một struct là một kiểu dữ liệu do lập trình viên tự định nghĩa, nó cũng cần được khai báo theo một cú pháp nhất định để compiler có thể hiểu được. Dưới đây là cú pháp để tạo ra một struct mới:

struct <name_of_new_type>
{
	<variables>;
};
Trong đó:

**struct** là từ khóa mà ngôn ngữ C++ cung cấp.  
name_of_new_type sẽ là tên của kiểu dữ liệu mới. Sau khi khai báo xong một struct, chúng ta có thể dùng tên struct để khai báo biến như những kiểu dữ liệu thông thường.  
variables là danh sách các biến dùng để lưu trữ dữ liệu phù hợp với yêu cầu lưu trữ dữ liệu của một đơn vị nào đó.  