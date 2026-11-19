# Tool_Copy-Google-Drive

Notebook Colab để copy dữ liệu giữa hai Google Drive trong **1 lần bấm chạy**:

- Copy 1 file riêng lẻ hoặc toàn bộ folder (kèm các thư mục con)
- Chấp nhận cả link Google Drive hoặc ID
- Hỗ trợ đầy đủ Shared Drive (`supportsAllDrives=True`)
- Bỏ qua file đã tồn tại và kiểm tra giới hạn dung lượng (`max_download_size_gb`)

## Mở trên Colab

https://colab.research.google.com/github/Vanquan99/Tool_Copy-Google-Drive/blob/main/tool_coppy_driver.ipynb

## Cách dùng

1. Mở [tool_coppy_driver.ipynb](tool_coppy_driver.ipynb) trên Colab.
2. Điền `source_link` (file/folder nguồn) và `dest_link` (folder đích).
3. Nhấn nút **Run** ở cell duy nhất (và cấp quyền Google Drive khi popup hiện ra).
