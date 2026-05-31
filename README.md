# Tool_Copy-Google-Drive

Google Colab notebook for copying data between two Google Drives. Hỗ trợ / Supports:

- Copy a single file / Copy một file riêng lẻ
- Copy an entire folder and subfolders / Copy toàn bộ folder và các thư mục con
- Work with Google Drive links or IDs / Làm việc với link Google Drive hoặc ID
- Support shared drives / Hỗ trợ shared drive

## Open on Colab / Mở trên Colab

Open the notebook directly with this link:

Mở trực tiếp notebook bằng link này:

https://colab.research.google.com/github/Vanquan99/Tool_Copy-Google-Drive/blob/main/tool_coppy_driver.ipynb

Or click the badge inside the notebook.

Hoặc nhấn badge trong notebook.

## How to use / Cách dùng

1. Open `tool_coppy_driver.ipynb` in Colab.
1. Mở `tool_coppy_driver.ipynb` trên Colab.
2. Run the `Input` cell and fill in:
2. Chạy cell `Input` và điền:
	- `dest_link`: destination folder link or ID / link hoặc ID thư mục đích
	- `source_link`: source file/folder link or ID / link hoặc ID file/folder nguồn
	- `from_page`, `to_page`: set to `0` to include all pages / để `0` nếu muốn lấy toàn bộ
	- `max_download_size_gb`: size limit in GB / giới hạn dung lượng
	- `exclude_str`: excluded strings, comma-separated / các chuỗi cần loại trừ, phân tách bằng dấu phẩy
3. Run the Google Drive authentication cell.
3. Chạy cell xác thực Google Drive.
4. Run the class definition cell.
4. Chạy cell định nghĩa class.
5. Run the last cell to start copying.
5. Chạy cell cuối để bắt đầu copy.

## Notes / Ghi chú

- If `source_link` is a file, the notebook copies that file directly. / Nếu `source_link` là file, notebook sẽ copy trực tiếp file đó.
- If `source_link` is a folder, the notebook creates a matching folder in the destination Drive and copies all contents inside. / Nếu `source_link` là folder, notebook sẽ tạo folder tương ứng ở Drive đích rồi copy toàn bộ nội dung bên trong.
- Google Drive permission is required when Colab asks for it. / Cần cấp quyền Google Drive khi Colab yêu cầu.

## Main file / Tệp chính

- `tool_coppy_driver.ipynb`: Colab notebook / notebook chạy trên Colab
