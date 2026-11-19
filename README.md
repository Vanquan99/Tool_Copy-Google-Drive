# Tool_Copy-Google-Drive (All-in-One)

Notebook Colab **1-cell duy nhất** giúp thao tác dữ liệu Google Drive tốc độ cao:

- **3 chế độ (`action`)**:
  - `Copy`: Sao chép file hoặc toàn bộ cây thư mục giữa 2 Google Drive (hỗ trợ cả Shared Drive).
  - `Check Size (Tính dung lượng)`: Đếm tổng số file, thư mục con và tổng dung lượng (MB/GB) của một hoặc nhiều folder/file.
  - `Unzip (Giải nén)`: Giải nén trực tiếp file `.zip` / `.tar` / `.tar.gz` trên Drive ra thư mục đích mà không cần tải về máy cá nhân.
- **Tối ưu hiệu năng**:
  - **Đa luồng (`workers = 1..8`)**: Copy/upload song song nhanh gấp 3–4 lần, mỗi luồng có kết nối HTTP riêng an toàn.
  - **Nhiều link nguồn cùng lúc**: Nhập nhiều link/ID vào `source_link` (ngăn cách bằng dấu phẩy `,`).
  - **Tự động thử lại (Auto-retry)**: Tự động retry khi Google API trả lỗi mạng hoặc giới hạn quota tạm thời.

## Mở trên Colab

https://colab.research.google.com/github/Vanquan99/Tool_Copy-Google-Drive/blob/main/tool_coppy_driver.ipynb

## Cách dùng

1. Mở [tool_coppy_driver.ipynb](tool_coppy_driver.ipynb) trên Colab.
2. Chọn `action`, điền `source_link` (và `dest_link` nếu dùng `Copy` / `Unzip`).
3. Bấm **Run** 1 lần duy nhất ở cell và cấp quyền Google Drive.
