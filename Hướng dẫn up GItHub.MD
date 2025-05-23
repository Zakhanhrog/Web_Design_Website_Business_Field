# 📘 HƯỚNG DẪN LÀM VIỆC NHÓM VỚI GIT (CHUẨN DOANH NGHIỆP)

> Áp dụng cho dự án web, app hoặc phần mềm nội bộ sử dụng GitHub/GitLab

---

## ✅ 1. QUY TẮC CHUNG

- Mỗi thành viên **không commit trực tiếp vào nhánh `main` hoặc `master`**
- Mỗi người làm việc trên **nhánh riêng (branch)** → tạo **Pull Request (PR)** để merge
- **Luôn cập nhật code mới nhất** từ `main` trước khi làm việc
- Commit rõ ràng, dễ hiểu, có mô tả đúng công việc

---

## 🏁 2. BẮT ĐẦU LÀM VIỆC

### 🔸 Clone repository (chỉ 1 lần duy nhất)
```bash
git clone https://github.com/ten-tai-khoan/ten-repo.git
cd ten-repo
```

---

## 🔧 3. QUY TRÌNH MỖI KHI LÀM VIỆC

### 3.1 Tạo nhánh mới từ `main`
```bash
git checkout main
git pull origin main           # Luôn cập nhật code mới nhất
git checkout -b feature/ten-chuc-nang
```
📌 Ví dụ: `feature/login-form`, `fix/navbar-error`

### 3.2 Code, commit
```bash
git add .
git commit -m "feat: thêm giao diện form đăng nhập"
```

#### 💡 Gợi ý format commit:
- `feat:` - Thêm chức năng mới
- `fix:` - Sửa lỗi
- `refactor:` - Cải tiến cấu trúc code
- `chore:` - Thay đổi không ảnh hưởng logic (ex: sửa README)

### 3.3 Push nhánh lên remote
```bash
git push origin feature/ten-chuc-nang
```

### 3.4 Tạo Pull Request (PR)
- Vào GitHub/GitLab → Pull Requests → New pull request
- Chọn nhánh `feature/...` của bạn → so với `main`
- Nhấn **Create pull request** và mô tả rõ ràng nội dung thay đổi

### 3.5 Review & Merge
- Thành viên khác hoặc leader sẽ **review code**
- Nếu đạt yêu cầu → **Merge vào `main`**
- Nếu cần sửa → bạn cập nhật lại code và push tiếp vào cùng branch

---

## 🔄 4. KHI CẦN CẬP NHẬT CODE MỚI NHẤT TỪ MAIN
```bash
git checkout main
git pull origin main
```
👉 Nên làm bước này **trước khi tạo branch mới hoặc khi bị xung đột code**

---

## 🌿 5. ĐẶT TÊN BRANCH CHUẨN
| Loại Branch | Ý nghĩa | Ví dụ |
|-------------|--------|--------|
| `feature/`  | Tính năng mới | `feature/add-product-page` |
| `fix/`      | Sửa lỗi | `fix/login-validation` |
| `refactor/` | Tối ưu code | `refactor/cart-service` |
| `hotfix/`   | Sửa lỗi khẩn cấp | `hotfix/payment-error` |

---

## 🛠️ 6. CÁC LỆNH GIT HỮU ÍCH
| Lệnh | Mục đích |
|------|----------|
| `git status` | Kiểm tra trạng thái file |
| `git branch` | Liệt kê nhánh hiện có |
| `git switch ten-nhanh` | Chuyển nhánh (hoặc dùng `checkout`) |
| `git log --oneline` | Xem lịch sử commit dạng rút gọn |
| `git stash` / `git stash pop` | Lưu tạm thời các thay đổi chưa commit |

---

## 📞 7. HỖ TRỢ KỸ THUẬT
Nếu gặp vấn đề liên quan đến Git hoặc quy trình làm việc:
- Email hỗ trợ: `support@tencongty.com`
- Trưởng nhóm kỹ thuật: `Nguyễn Văn A`

---

**Hãy làm đúng quy trình để tránh xung đột, tiết kiệm thời gian và làm việc hiệu quả hơn!** 🚀
