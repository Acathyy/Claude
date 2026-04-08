---
name: Cấu trúc chi tiết SRS chuẩn GTM – VNPT
description: Tài liệu hướng dẫn chuẩn đặc tả yêu cầu phần mềm (SRS) cho các dự án tại VNPT AI.
---
# Cấu trúc chi tiết SRS chuẩn GTM – VNPT

## MỤC LỤC
1. [Trang bìa & Thông tin tài liệu](#1)
2. [Tổng quan hệ thống](#2)
3. [Nội dung](#3)
4. [Yêu cầu phi chức năng](#4)
5. [Điều kiện nghiệm thu hệ thống](#5)
---

## 1. TRANG BÌA & THÔNG TIN TÀI LIỆU {#1}

### Trang bìa (bắt buộc)
```
Logo VNPT (góc trên trái)
TẬP ĐOÀN BƯU CHÍNH VIỄN THÔNG VIỆT NAM (góc trên phải)
CÔNG TY VNPT AI (góc trên phải)
[Tên sản phẩm]
TÀI LIỆU ĐẶC TẢ YÊU CẦU PHẦN MỀM
Mã số: [Tên sản phẩm]_SRS
Phiên bản: x.x
Ngày hiệu lực: DD/MM/YYYY
```

### LỊCH SỬ THAY ĐỔI
| STT | Phiên bản | Người thực hiện | Người xem xét | Người phê duyệt | Ngày hiệu lực | Nội dung thay đổi |
---

## 2. TỔNG QUAN HỆ THỐNG {#2}

### 2.1 Mục đích
Mô tả lý do tồn tại của tài liệu. Trả lời: Tài liệu này phục vụ ai? Dùng để làm gì? Thay đổi trong tài liệu tác động như thế nào?
_Mẫu:_
> Tài liệu này nhằm mục đích đặc tả chi tiết yêu cầu chức năng của sản phẩm [Tên sản phẩm]. Tài liệu là cơ sở và là kết quả đầu vào cho các tài liệu thiết kế chi tiết, kịch bản kiểm thử hệ thống. Mỗi yêu cầu thay đổi trong tài liệu này sẽ ảnh hưởng đến kết quả phân tích, thiết kế, lập trình và các kịch bản kiểm tra liên quan đến sản phẩm

### 2.2 Phạm vi hệ thống
- Mô tả các chức năng / module được xây dựng trong dự án này

### 2.3 Tài liệu liên quan
| STT | Tên tài liệu | Tên file | 
|-----|-------------|-----------|
| 1 | Biên bản khảo sát nghiệp vụ | | 
| 2 | Tài liệu kiến trúc hệ thống | | 

### 2.4 Giải thích từ ngữ và các chữ viết tắt
| Thuật ngữ | Ý nghĩa |
|-------------------------|-----------|
| SRS | Software Requirements Specification |
| GTM | Go-To-Market |
| FR | Functional Requirement – Yêu cầu chức năng |
| NFR | Non-Functional Requirement – Yêu cầu phi chức năng |
| UC | Use Case |
| BA | Business Analyst |
| [Thuật ngữ dự án] | [Giải thích] |
---

## 3. NỘI DUNG {#3}

### 3.1 Tổng quan hệ thống
####3.1.1 Phát biểu bài toán 
Phát biểu ngắn gọn bối cảnh và bài toán mà [Tên sản phẩm] xử lý
####3.1.2 Mục tiêu và phạm vi hệ thống 
Phát biểu ngắn gọn mục tiêu hệ thống, các phương thức giao tiếp với hệ thống
####3.1.3 Mô hình hệ thống 
Mô hình  hóa tổng thể từ tính năng và phương thức giao tiếp đã mô tả ở trên

### 3.2 Đặc tả yêu cầu chức năng hệ thống
Tổ chức theo **module** hoặc **nhóm chức năng**. Mỗi module có một mục riêng (3.2.1, 3.2.2...).
####3.2.1. [Tên chức năng] 
#####3.2.1.1. Mô tả tóm tắt
Mô tả ngắn gọn chức năng 
#####3.2.1.2. Yêu cầu giao diện
Chụp ảnh màn hình tương ứng với chức năng (nếu có)
#####3.2.1.3. SRS[xx]: [Tên use case]
Mô tả các tình huống sử dụng 
Thực hiện tương tự cho các chức năng còn lại của hệ thống

## 4. YÊU CẦU PHI CHỨC NĂNG {#4}

### 4.1 Yêu cầu bảo mật, phân quyền người dùng
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|
| YC001 | Phân quyền cho người dùng khi đăng nhập chỉ nhìn thấy thông tin của chính tài khoản đó | Người dùng có tài khoản đăng nhập chỉ nhìn thấy các thông tin tài khoản, thông tin liên quan đến việc sử dụng các dịch vụ, gói cước của sản phẩm của chính người dùng đó | 

### 4.2 Yêu cầu ghi log hệ thống
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|
| YC00x | Có cơ chế rotate log, cấu hình log, quản lý log | Log giao dịch được lưu trữ và quản lý trong database |

### 4.3 Yêu cầu sao lưu và khôi phục dữ liệu 
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.4 Yêu cầu về tính khả dụng
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.5 Yêu cầu về tính ổn định
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.6 Yêu cầu về hiệu năng
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|
### 4.7 Yêu cầu về tính hỗ trợ
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.8 Yêu cầu các ràng buộc thiết kế
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.9 Yêu cầu về giao tiếp
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.10 Các yêu cầu về tài liệu người dùng và hỗ trợ trực tuyến
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.11 Yêu cầu về các thành phần mua ngoài
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.12 Các yêu cầu pháp lý, bản quyền và ghi chú khác
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

### 4.13 Các tiêu chuẩn áp dụng
| Mã YC| Yêu cầu | Đặc tả |
|----|---------|-------------|

---

## 5. Điều kiện nghiệm thu hệ thống {#5}
Mô tả các điều kiện nghiệm thu hệ thống


