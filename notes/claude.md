# Ghi chú: Dùng Claude Code trong repo này

## 1. Mở repo
Vào thư mục repo trước khi chạy Claude Code:

```bash
cd /Users/drson/Documents/GitHub/stargazers-log
```

## 2. Đọc cấu trúc thư mục
Yêu cầu Claude liệt kê file/thư mục, hoặc tự chạy:

```bash
find . -not -path './.git*' | sort
```

## 3. Tạo file
Nhờ Claude tạo file mới (ví dụ `notes/xyz.md`), Claude sẽ dùng công cụ Write để ghi nội dung. Có thể yêu cầu trực tiếp: "tạo file ... với nội dung ...".

## 4. Sửa file
Nhờ Claude chỉnh sửa nội dung file có sẵn (Claude dùng công cụ Edit, không ghi đè toàn bộ file trừ khi cần). Nên mô tả rõ đoạn cần sửa và nội dung mong muốn.

## 5. Kiểm tra thay đổi
Trước khi commit, xem lại các thay đổi:

```bash
git status
git diff
```

## 6. Commit
Chỉ commit khi được yêu cầu rõ ràng. Ví dụ:

```bash
git add <file>
git commit -m "Mô tả ngắn gọn thay đổi"
```

## 7. Push
Chỉ push khi được yêu cầu rõ ràng, thường sau khi đã commit:

```bash
git push
```
