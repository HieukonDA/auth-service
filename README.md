# AuthService

## Mô tả
Dịch vụ xác thực và ủy quyền cho hệ thống thương mại điện tử, được xây dựng bằng ASP.NET Core Web API.

## Công nghệ sử dụng
- **Framework:** ASP.NET Core 8.0
- **Architecture:** Web API RESTful
- **Authentication:** JWT (JSON Web Tokens)
- **Database:** Entity Framework Core
- **Language:** C# .NET

## Chức năng chính
- Đăng ký tài khoản người dùng
- Đăng nhập và xác thực
- Quản lý JWT tokens
- Phân quyền người dùng (Role-based)
- Reset mật khẩu

## Cài đặt và chạy

### Yêu cầu hệ thống
- .NET 8.0 SDK
- SQL Server hoặc PostgreSQL

### Chạy dự án
```bash
# Khôi phục packages
dotnet restore

# Chạy migration database
dotnet ef database update

# Chạy ứng dụng
dotnet run
```

### API Endpoints
- `POST /api/auth/register` - Đăng ký tài khoản
- `POST /api/auth/login` - Đăng nhập
- `POST /api/auth/refresh` - Refresh token
- `POST /api/auth/logout` - Đăng xuất

## Cấu hình
Cập nhật file `appsettings.json` với thông tin database và JWT settings.

## Môi trường phát triển
- **IDE:** Visual Studio 2022 / VS Code
- **Version Control:** Git
- **API Testing:** Postman/Swagger UI