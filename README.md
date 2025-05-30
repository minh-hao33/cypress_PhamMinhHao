# Cypress End-to-End Testing Exercise

## Mục tiêu
- Hiểu và thực hành các kịch bản kiểm thử tự động end-to-end phổ biến.
- Sử dụng Cypress để kiểm tra các chức năng của trang web mẫu [https://www.saucedemo.com](https://www.saucedemo.com).
- Thực hiện các kịch bản kiểm tra giao diện người dùng, đăng nhập, tìm kiếm, thêm/xóa sản phẩm trong giỏ hàng, và quy trình thanh toán.

---

## Yêu cầu
- Đã cài đặt Node.js (phiên bản 14 hoặc cao hơn).
- Đã cài đặt Visual Studio Code hoặc một trình soạn thảo mã khác.
- Truy cập được trang web mẫu: [https://www.saucedemo.com](https://www.saucedemo.com).
- Cài đặt Cypress trong dự án.

---

## Hướng dẫn cài đặt Cypress
1. Tạo thư mục dự án và khởi tạo npm:
    ```bash
    mkdir cypress-exercise
    cd cypress-exercise
    npm init -y
    ```
    Cài đặt Cypress:

    ```bash
    npm install cypress --save-dev
    ```
    Mở Cypress:

    ```bash
    npx cypress open
    ```
Lệnh này sẽ tạo cấu trúc thư mục và các tệp mẫu trong thư mục cypress.

## Chạy các bài kiểm thử

**Mở Cypress Test Runner**

   Khi chạy lệnh:
   ```bash
   npx cypress open
   ```
Cửa sổ Cypress Test Runner sẽ hiện ra, hiển thị danh sách các file kiểm thử .cy.js trong thư mục cypress/e2e/.

Chọn file kiểm thử cần chạy

- login_spec.cy.js — kiểm thử chức năng đăng nhập.

- cart_spec.cy.js — kiểm thử giỏ hàng, sắp xếp, xóa sản phẩm và thanh toán.

Khi chọn một file, Cypress sẽ tự động chạy tất cả các test case trong file đó và hiển thị kết quả ngay trên màn hình.

### Quan sát kết quả kiểm thử

- Bạn có thể xem trạng thái Pass/Fail của từng bước kiểm thử trong giao diện Test Runner.

- Cypress tự động chụp ảnh màn hình khi test bị lỗi.

- Nếu bạn muốn chạy kiểm thử nhanh qua terminal mà không cần mở giao diện, sử dụng lệnh:

    ```bash
    npx cypress run
    ```
Kết quả kiểm thử sẽ được in trực tiếp ra terminal.

