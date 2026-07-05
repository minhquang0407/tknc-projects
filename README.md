# Đồ án Cuối kỳ: Ứng dụng Phân tích Thống kê Nhiều chiều (Multivariate Statistics)

Chào mừng bạn đến với kho lưu trữ mã nguồn và dữ liệu dự phòng cho đồ án môn học **Thống kê Nhiều chiều**. Kho lưu trữ này được thiết lập nhằm mục đích minh bạch hóa quá trình nghiên cứu.

## 📊 Tổng quan (Overview)

Đồ án ứng dụng các kỹ thuật Thống kê đa biến chuyên sâu để phân tích và khai phá tri thức trên 3 bộ dữ liệu độc lập thuộc 3 lĩnh vực khác nhau: Y tế, Xã hội học (Giáo dục), và Cơ học.

*   **Dữ liệu 1: Sleep Health and Lifestyle** (Y tế) - Phân tích kiểu hình rối loạn giấc ngủ và nguy cơ tim mạch.
*   **Dữ liệu 2: Student Habits vs Academic Performance** (Giáo dục) - Đánh giá mức độ đồng biến giữa thói quen sinh hoạt và thành quả học tập.
*   **Dữ liệu 3: NASA C-MAPSS Turbofan Engine** (Cơ học) - Xử lý tín hiệu chuỗi thời gian, lọc nhiễu động học và phân tích sự thoái hóa của động cơ.

## 🛠 Phương pháp Thống kê sử dụng

Dự án triển khai cài đặt các thuật toán thống kê bằng ngôn ngữ **R**, bao gồm:
*   Phân tích thành phần chính (PCA - Principal Component Analysis)
*   Phân tích nhân tố khám phá (EFA - Exploratory Factor Analysis)
*   Phân tích phương sai nhiều chiều (MANOVA)
*   Hồi quy đa biến (Multivariate Linear Regression)
*   Phân cụm K-Means
*   Bộ lọc Kalman (Kalman Filter) và Mô hình hỗn hợp Gauss (GMM)
*   Tính toán khoảng cách Mahalanobis và Hotelling $T^2$

## 📁 Cấu trúc Thư mục

Kho lưu trữ này được cấu trúc tương ứng với file nén nộp cho Giảng viên:

```text
📦 tknc-projects
 ┣ 📂 data/               # Chứa 3 bộ dữ liệu gốc định dạng CSV
 ┃ ┣ 📜 Sleep_health_and_lifestyle_dataset.csv
 ┃ ┣ 📜 student_performance.csv
 ┃ ┗ 📜 cmapss_FD001.txt (C-MAPSS)
 ┃ ┗ 📜 cmapss_FD001.txt (C-MAPSS)
 ┣ 📂 code/                    # Mã nguồn xử lý
 ┃ ┣ 📜 data1.Rmd      # Source code data Sleep_health_and_lifestyle_dataset viết bằng R Markdown
 ┃ ┣ 📜 data2.Rmd      # Source code data student_performance viết bằng R Markdown
 ┃ ┣ 📜 data3.Rmd      # Source code data CMAPSS bằng R Markdown
 ┃ ┗ 📜 data1.html     # Kết quả thực thi chi tiết data Sleep_health_and_lifestyle_dataset  (Compiled output)
 ┃ ┗ 📜 data2.html     # Kết quả thực thi chi tiết data student_performance (Compiled output)
 ┃ ┗ 📜 data3.html     # Kết quả thực thi chi tiết data CMAPSS (Compiled output)
 ┣ 📜 DoAn.pdf           # File báo cáo gốc định dạng PDF
 ┗ 📜 README.md                # File giới thiệu này
```

## 🚀 Hướng dẫn thực thi

Để chạy lại mã nguồn của dự án trên máy cá nhân, bạn cần cài đặt **R** và **RStudio**.

1. Clone kho lưu trữ này về máy:
   ```bash
   git clone https://github.com/minhquang0407/tknc-projects.git
   ```
2. Mở file `code/analysis_tknc.Rmd` bằng RStudio.
3. Cài đặt các packages cần thiết (nếu RStudio yêu cầu): `ggplot2`, `dplyr`, `factoextra`, `MASS`, `FKF`, v.v.
4. Chạy từng chunk code hoặc nhấn nút **Knit** để biên dịch lại toàn bộ báo cáo sang định dạng HTML/PDF.

---
*Kho lưu trữ này là minh chứng đính kèm cho Đồ án Thống kê Nhiều chiều. Nếu có bất kỳ sự cố nào với file nén nộp qua hệ thống trường, xin vui lòng đối chiếu trực tiếp tại đây.*
