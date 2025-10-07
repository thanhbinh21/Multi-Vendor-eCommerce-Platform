# Web Ecommore

Một ứng dụng web thương mại điện tử mẫu.

## Tổng quan
- Backend: Spring Boot (Java), MySQL, Spring Security, JWT, Java Mail Sender  
- Frontend: React + TypeScript (Redux Toolkit, MUI, Tailwind, Formik, Yup, React Router, Axios, React Chart)  
- Thanh toán: Razorpay (dành cho học viên Ấn Độ) và Stripe (quốc tế)

## Yêu cầu
- Java 21+
- Maven (sử dụng wrapper: [mvnw](mvnw))
- MySQL (cấu hình trong [src/main/resources/application.properties](src/main/resources/application.properties))

## Cách chạy
1. Cấu hình cơ sở dữ liệu và các biến môi trường cần thiết trong [src/main/resources/application.properties](src/main/resources/application.properties).  
2. Chạy ứng dụng:
   - Trên Windows: mvnw.cmd spring-boot:run
   - Trên macOS/Linux: ./mvnw spring-boot:run
   Lớp chính: [`com.binhse.WebEcommoreApplication`](src/main/java/com/binhse/WebEcommoreApplication.java)

## Xây dựng & Kiểm thử
- Build: ./mvnw package
- Kiểm thử: ./mvnw test (xem [`com.binhse.WebEcommoreApplicationTests`](src/test/java/com/binhse/WebEcommoreApplicationTests.java))

## Tệp quan trọng
- Cấu hình ứng dụng: [src/main/resources/application.properties](src/main/resources/application.properties)  
- POM & phụ thuộc: [pom.xml](pom.xml)  
- Tài liệu bổ sung: [HELP.md](HELP.md)

## Ghi chú
- Frontend (React) được phát triển tách rời; hướng dẫn chạy frontend nằm trong repository frontend (nếu có).
- Cập nhật các giá trị nhạy cảm (API keys, mật khẩu DB) qua biến môi trường, không commit vào git.
