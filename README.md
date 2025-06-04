# TinyDB – Cơ sở dữ liệu nhỏ gọn, dễ dùng, dạng tài liệu

**TinyDB** là một cơ sở dữ liệu dạng tài liệu (document-oriented) siêu nhẹ, được viết hoàn toàn bằng Python, không cần cài thêm thư viện ngoài. Dữ liệu được lưu trong file JSON và bạn có thể truy vấn bằng cú pháp Python rất trực quan.

---

## ✨ Tính năng

- 📝 Lưu dữ liệu dưới dạng tài liệu (document) như MongoDB
- 🧩 Viết 100% bằng Python, không cần cài thêm gói nào khác
- 💾 Lưu dữ liệu trong file JSON thuần
- 🔍 Truy vấn linh hoạt bằng cách sử dụng biểu thức Python
- 📚 Hỗ trợ nhiều loại lưu trữ: file, bộ nhớ RAM, hoặc tùy chỉnh
- 🧪 Phù hợp cho các ứng dụng nhỏ, công cụ cá nhân, demo, học tập

---

## 🚀 Cài đặt

Cài đặt qua `pip`:

```bash
pip install tinydb

🧪 Cách sử dụng cơ bản
python
Sao chép
Chỉnh sửa
from tinydb import TinyDB, Query

# Khởi tạo database lưu trong file 'db.json'
db = TinyDB('db.json')

# Thêm một tài liệu mới
db.insert({'name': 'Nam', 'age': 20})

# Tạo truy vấn
User = Query()

# Tìm các tài liệu có tên là 'Nam'
results = db.search(User.name == 'Nam')

print(results)
📚 Tài liệu
Bạn có thể xem tài liệu chi tiết và các ví dụ nâng cao tại:
👉 https://tinydb.readthedocs.io/

✅ Các phiên bản Python được hỗ trợ
TinyDB hỗ trợ Python từ phiên bản 3.7 trở lên.

📌 Khi nào nên dùng TinyDB?
TinyDB phù hợp với:

Các ứng dụng nhỏ, công cụ cá nhân

Lưu cấu hình hoặc dữ liệu đơn giản

Ứng dụng desktop, CLI, phần mềm nhúng

Mục đích học tập, thử nghiệm nhanh ý tưởng

Không khuyến khích dùng TinyDB nếu bạn cần xử lý dữ liệu lớn, truy cập đồng thời cao, hoặc các truy vấn phức tạp. Trong trường hợp đó, bạn nên dùng các hệ cơ sở dữ liệu như PostgreSQL, MongoDB,...

🤝 Đóng góp
Bạn tìm thấy lỗi hoặc muốn đề xuất tính năng?
Hãy mở issue hoặc gửi pull request! TinyDB luôn chào đón sự đóng góp từ cộng đồng.

Xem thêm hướng dẫn đóng góp tại:
👉 https://tinydb.readthedocs.io/en/latest/contributing.html

📄 Giấy phép
TinyDB được phát hành theo giấy phép MIT.
Xem chi tiết trong file LICENSE
