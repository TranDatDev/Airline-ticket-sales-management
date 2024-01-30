# Airline-ticket-sales-management

## Quản lý bán vé máy bay

[![made-with](https://img.shields.io/badge/Made%20with-WinForms-1f425f.svg)](https://learn.microsoft.com/vi-vn/dotnet/desktop/winforms/?view=netframeworkdesktop-4.8)
[![language](https://img.shields.io/badge/Language-C%23_.NET-1f425f.svg)](https://learn.microsoft.com/vi-vn/dotnet/desktop/winforms/?view=netframeworkdesktop-4.8)

![Static Badge](https://img.shields.io/badge/Database-Microsoft_SQL_Server-blue?logo=microsoftsqlserver)

![Static Badge](https://img.shields.io/badge/Architecture-3%20Layers-green)

![Static Badge](https://img.shields.io/badge/Structure-GUI%20BLL%20DAL-green)

![Static Badge](https://img.shields.io/badge/License-MIT-green)
### Giao diện đồ họa người dùng (GUI)

- Giao diện đồ họa người dùng có nhiệm vụ giao tiếp với NGƯỜI DÙNG
- Bao gồm các dạng giao diện như Form, TextBox, DataGridView,...
- Thực hiện các công việc hiển thị (nhập xuất, thông báo,...) từ dữ liệu đã được kiểm tra từ BLL

- Hướng dẫn đặt tên cho thành phần

[Cách thức đặt tên thành phần viết tắt GUI](GUI-naming-convention.txt)

thành phần | thuộc tính | TÊN
-----------|------------|------------
Text Box   | User Name  | txtUserName

### Lớp Nghiệp Vụ Hợp Lý (BLL)

- Lớp nghiệp vụ hợp lý có nhiệm vụ kiểm tra tính hợp lý nhập xuất
- Bao gồm các dạng hàm logic, hàm tính toán, ... và DTO
- Thực hiện thao tác kiểm tra rằng buộc, tính toàn vẹn hợp lý,... trước khi gửi về cho DAL hoặc GUI
- Thư mục DTO (đối tượng truyền dữ liệu) với tên file là [Đối_Tượng]DTO.cs

[Cách thức đặt tên thành phần BLL](BLL-DAL-naming-convention.txt)

thành phần | thuộc tính | TÊN
-----------|------------|-----------
logic      | Login      | LogicLogin
Calculate  | People     | CalcPeople


### Lớp Truy Vấn Dữ Liệu (DAL)

- Lớp truy vấn dữ liệu có nhiệm vụ truy cập cơ sở dữ liệu
- Bao gồm các dạng câu lệnh phương thức sql để truy vấn
- Thực hiện truy vấn và tổng kết dữ liệu trước khi gửi về cho BLL
- thư mục DAO (đối tượng truy vấn dữ liệu) với tên file là [Đối_Tượng]DAO.cs

[Cách thức đặt tên thành phần DAL](BLL-DAL-naming-convention.txt)