# WEATHER APP - THỰC HÀNH GIT VÀ GITHUB

## Thông tin sinh viên

- Họ và tên: Nguyễn Ngọc Thắng
- Mã sinh viên: DTC245180018
- Repository: https://github.com/dtc245180018-gif/weather-app

---

## Giới thiệu

Đây là project `weather-app` được sử dụng để thực hành Git và GitHub.

Project ban đầu gồm các file JavaScript phục vụ cho việc xây dựng ứng dụng thời tiết. Trong quá trình thực hành Git, em tiếp tục bổ sung giao diện HTML, CSS và thực hiện các thao tác quản lý phiên bản như:

- Theo dõi thay đổi của file.
- Tạo commit.
- Push code lên GitHub.
- Kiểm tra lịch sử commit.
- Sửa đổi giao diện.
- Tạo commit sai để mô phỏng lỗi.
- Hoàn tác commit bằng `git revert`.

---

## Cấu trúc project

```text
weather-app/
│
├── README.md
├── index.html
├── style.css
├── weather.js
├── search.js
├── favorite.js
└── scratch.txt
````

### Mô tả các file

* `index.html`: Giao diện HTML và phần giới thiệu cá nhân.
* `style.css`: Định dạng giao diện của trang.
* `weather.js`: File JavaScript của chức năng thời tiết.
* `search.js`: File xử lý chức năng tìm kiếm.
* `favorite.js`: File xử lý chức năng yêu thích.
* `scratch.txt`: File được tạo trong quá trình phát triển project.
* `README.md`: Tài liệu giới thiệu và mô tả quá trình thực hành.

---

# Quá trình phát triển project

## 1. Khởi tạo cấu trúc dự án

Project ban đầu được tạo với các file phục vụ cho Weather App.

Một số commit đầu của project gồm:

```text
Khởi tạo cấu trúc dự án
Tạo search.js và cập nhật weather.js
Thêm tính năng favorite và xóa sun icon
```

Qua các commit này, em thực hành việc tạo file, chỉnh sửa file và lưu lại từng phiên bản bằng Git.

---

## 2. Tạo cấu trúc HTML và CSS

Trong phần thực hành tổng hợp, em bổ sung:

```text
index.html
style.css
```

Sau đó thực hiện commit:

```text
Initial structure
```

Các lệnh đã sử dụng:

```bash
git add index.html style.css
git commit -m "Initial structure"
git push
```

---

## 3. Thêm phần giới thiệu

Em bổ sung phần giới thiệu vào `index.html`.

Commit:

```text
Add introduction section
```

Lệnh thực hiện:

```bash
git add index.html
git commit -m "Add introduction section"
git push
```

---

## 4. Thêm CSS cho phần giới thiệu

Em chỉnh sửa `style.css` để định dạng phần giới thiệu.

Commit:

```text
Style introduction section
```

Lệnh:

```bash
git add style.css
git commit -m "Style introduction section"
git push
```

---

## 5. Mô phỏng một commit sai

Để thực hành việc hoàn tác phiên bản, em cố tình thêm CSS sai:

```css
.introduction {
    display: none;
}
```

Thay đổi này làm phần giới thiệu bị ẩn.

Sau đó thực hiện:

```bash
git add style.css
git commit -m "Wrong CSS change"
git push
```

Commit được tạo:

```text
Wrong CSS change
```

---

## 6. Hoàn tác commit sai bằng Git Revert

Do commit sai đã được push lên GitHub nên em không sử dụng `reset --hard` để xóa lịch sử.

Thay vào đó em sử dụng:

```bash
git revert HEAD --no-edit
```

Sau đó:

```bash
git push
```

Git tạo một commit mới:

```text
Revert "Wrong CSS change"
```

Sau khi revert:

* CSS sai được loại bỏ.
* Phần giới thiệu hiển thị lại bình thường.
* Commit sai vẫn được giữ trong lịch sử.
* Các commit trước đó không bị mất.

Đây là cách an toàn hơn khi thay đổi đã được đưa lên remote repository.

---

# Một số lệnh Git đã sử dụng

## Kiểm tra trạng thái

```bash
git status
```

## Kiểm tra lịch sử

```bash
git log --oneline
```

## Xem thay đổi

```bash
git diff
```

## Đưa file vào Staging Area

```bash
git add <file>
```

## Tạo commit

```bash
git commit -m "Commit message"
```

## Kiểm tra remote

```bash
git remote -v
```

## Đẩy code lên GitHub

```bash
git push
```

## Lấy thay đổi từ remote

```bash
git pull
```

## Hoàn tác một commit

```bash
git revert HEAD
```

---

# Một số commit chính

Trong quá trình phát triển repository có các commit tiêu biểu:

```text
Khởi tạo cấu trúc dự án
Tạo search.js và cập nhật weather.js
Thêm tính năng favorite và xóa sun icon
Initial structure
Add introduction section
Style introduction section
Wrong CSS change
Revert "Wrong CSS change"
```

Ngoài ra repository còn có các commit cập nhật tài liệu `README.md`.

Có thể xem toàn bộ lịch sử bằng:

```bash
git log --oneline
```

---

# Kết quả đạt được

Qua project này em đã thực hành được:

* Tạo và quản lý repository Git.
* Theo dõi trạng thái file.
* Sử dụng Staging Area.
* Tạo nhiều commit.
* Kiểm tra lịch sử bằng `git log`.
* Kiểm tra thay đổi bằng `git diff`.
* Kết nối local repository với GitHub.
* Push code lên remote.
* Pull thay đổi từ remote.
* Thực hành sửa giao diện HTML/CSS.
* Hoàn tác commit sai bằng `git revert`.
* Hiểu được cách Git lưu lại lịch sử phát triển của project.

---
