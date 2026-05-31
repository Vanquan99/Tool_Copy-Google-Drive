# Tool_Copy-Google-Drive

Notebook Colab để copy dữ liệu giữa hai Google Drive. Hỗ trợ:

- Copy một file riêng lẻ
- Copy toàn bộ folder và các thư mục con
- Làm việc với link Google Drive hoặc ID
- Hỗ trợ shared drive

## Mở trên Colab

Mở trực tiếp notebook bằng link này:

https://colab.research.google.com/github/Vanquan99/Tool_Copy-Google-Drive/blob/main/tool_coppy_driver.ipynb

Hoặc nhấn badge trong notebook.

## Cách dùng

1. Mở `tool_coppy_driver.ipynb` trên Colab.
2. Chạy cell `Input` và điền:
	- `dest_link`: link hoặc ID thư mục đích
	- `source_link`: link hoặc ID file/folder nguồn
	- `from_page`, `to_page`: để `0` nếu muốn lấy toàn bộ
	- `max_download_size_gb`: giới hạn dung lượng
	- `exclude_str`: các chuỗi cần loại trừ, phân tách bằng dấu phẩy
3. Chạy cell xác thực Google Drive.
4. Chạy cell định nghĩa class.
5. Chạy cell cuối để bắt đầu copy.

## Ghi chú

- Nếu `source_link` là file, notebook sẽ copy trực tiếp file đó.
- Nếu `source_link` là folder, notebook sẽ tạo folder tương ứng ở Drive đích rồi copy toàn bộ nội dung bên trong.
- Cần cấp quyền Google Drive khi Colab yêu cầu.

## Tệp chính

- `tool_coppy_driver.ipynb`: notebook chạy trên Colab
