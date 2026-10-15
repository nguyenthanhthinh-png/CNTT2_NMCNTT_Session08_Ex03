# Hướng dẫn cài đặt Visual Studio Code (VS Code)

## 1. Mục tiêu

Sau khi hoàn thành hướng dẫn này, bạn có thể:

-   Tải và cài đặt VS Code.
-   Mở Terminal và chạy thử một chương trình Python.
-   Phân biệt văn bản giải thích với câu lệnh cần nhập.
-   Theo dõi tiến độ bằng danh sách kiểm tra.

## 2. Chuẩn bị

Bạn cần có:

-   Máy tính kết nối Internet.
-   Quyền cài đặt phần mềm trên máy tính.
-   Python nếu muốn chạy chương trình Python trong VS Code.

Tải VS Code tại: <https://code.visualstudio.com/>

## 3. Các bước cài đặt

### Bước 1: Tải và cài đặt VS Code

1.  Mở trang tải xuống chính thức của VS Code.
2.  Chọn phiên bản phù hợp với hệ điều hành.
3.  Mở tệp cài đặt vừa tải và làm theo hướng dẫn trên màn hình.
4.  Khởi động VS Code sau khi cài đặt xong.

### Bước 2: Mở Terminal trong VS Code

Trên thanh menu, chọn **Terminal → New Terminal**.

Trong Terminal, bạn có thể kiểm tra phiên bản Python bằng lệnh sau:

``` powershell
python --version
```

Nếu lệnh trên không hoạt động trên Windows, hãy thử:

``` powershell
py --version
```

> Đây là các lệnh cần nhập vào Terminal. Không nhập dấu ba backtick bao
> quanh khối code.

### Bước 3: Tạo và chạy thử chương trình Python

1.  Tạo một thư mục cho bài thực hành.
2.  Trong VS Code, mở thư mục đó bằng **File → Open Folder**.
3.  Tạo tệp `hello.py`.
4.  Nhập đoạn mã Python sau:

``` python
# Chương trình Python đầu tiên
student_name = "Sinh viên PTIT"
course = "Nhập môn Công nghệ thông tin"

def greet(name, subject):
    """In lời chào và tên môn học."""
    message = f"Xin chào, {name}!"
    print(message)
    print(f"Môn học: {subject}")

greet(student_name, course)
```

Trong ví dụ này, `student_name`, `course` và `message` là các tên biến.
Inline Code giúp làm nổi bật tên biến trong câu giải thích mà không tạo
một khối code riêng.

Chạy chương trình bằng cách mở Terminal tại thư mục chứa tệp và nhập:

``` powershell
python hello.py
```

Kết quả dự kiến:

``` text
Xin chào, Sinh viên PTIT!
Môn học: Nhập môn Công nghệ thông tin
```

Nếu máy tính không nhận lệnh `python`, hãy thử `py hello.py` trên
Windows.

## 4. Bảng so sánh StackEdit và VS Code

  -----------------------------------------------------------------------
  Tiêu chí                StackEdit               VS Code
  ----------------------- ----------------------- -----------------------
  Cách sử dụng            Soạn Markdown trực tiếp Ứng dụng cài trên máy
                          trên trình duyệt        tính

  Xem trước Markdown      Có khung xem trước trực Có chức năng xem trước
                          quan                    Markdown

  Làm việc ngoại tuyến    Có giới hạn tùy cách    Phù hợp để làm việc với
                          lưu và đồng bộ          tệp cục bộ

  Viết mã lập trình       Phù hợp tài liệu        Hỗ trợ nhiều ngôn ngữ
                          Markdown, không phải    và tiện ích mở rộng
                          IDE chính               

  Phù hợp nhất            Soạn và xem trước tài   Phát triển phần mềm và
                          liệu nhanh              quản lý dự án mã nguồn
  -----------------------------------------------------------------------

## 5. Checklist kiểm tra tiến độ cài đặt

Đánh dấu từng mục sau khi hoàn thành:

-   [ ] Đã tải VS Code từ trang chính thức.
-   [ ] Đã cài đặt và mở được VS Code.
-   [ ] Đã mở được Terminal trong VS Code.
-   [ ] Đã kiểm tra phiên bản Python.
-   [ ] Đã tạo tệp `hello.py`.
-   [ ] Đã chạy chương trình và xem kết quả.
-   [ ] Đã biết cách mở chế độ xem trước Markdown.

## 6. Escape các ký tự Markdown

Một số ký tự có ý nghĩa đặc biệt trong Markdown. Đặt dấu gạch chéo ngược
`\\` trước ký tự cần hiển thị nguyên dạng để tránh việc Markdown diễn
giải nó thành cú pháp định dạng.

Ví dụ:

-   Viết `\\*` để hiển thị ký tự `*`.
-   Viết `\\#` để hiển thị ký tự `#`.
-   Viết `\\\\` để hiển thị một dấu gạch chéo ngược.

## 7. Kết luận

Sau khi hoàn thành checklist, bạn đã thiết lập môi trường VS Code cơ bản
và chạy thử một chương trình Python. Khi soạn tài liệu bằng Markdown,
hãy dùng Inline Code cho tên biến hoặc lệnh ngắn, Code Block cho đoạn mã
nhiều dòng, bảng để so sánh và Task List để theo dõi tiến độ.
