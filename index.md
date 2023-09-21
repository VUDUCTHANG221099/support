- Git là một hệ thống kiểm soát phiên bản.
- Git giúp bạn theo dõi các thay đổi về mã.
- Git được sử dụng để cộng tác về mã.
- Check Version: git --version

1. Configure Git

- git config --global user.name "w3schools-test"
- git config --global user.email "test@w3schools.com"
- Lưu ý: Sử dụng global để đặt tên người dùng và e-mail cho mọi kho lưu trữ trên máy tính của bạn.
- Nếu bạn chỉ muốn đặt tên người dùng/e-mail cho kho lưu trữ hiện tại, bạn có thể xóaglobal

2. Initialize Git

- git init

3. Check status

- git status
- git status --short
- [?? - Tập tin không bị theo dõi
  A - Tập tin được thêm vào giai đoạn
  M - Tập tin đã sửa đổi
  D - Tập tin đã xóa]

4. Git Staging Environment

- git add files
- git add --all
- git add -A
- git add .

5. Git Commit

- git commit -m "message"
- git commit -a -m "message"

6. Git Commit Log

- Để xem lịch sử các cam kết của một kho lưu trữ, bạn có thể sử dụng log lệnh:
- git log

7. Git Help

- git command -help - Xem tất cả các tùy chọn có sẵn cho lệnh cụ thể
- git help --all - Xem tất cả các lệnh có thể

8. New Git Branch

- git branch NewBranch

9. List Branch

- git branch

10. Delete Branch

- git branch -d NameBranch

11. Change Branch

- git checkout Branch
- Lưu ý: Sử dụng -b tùy chọn bật checkout sẽ tạo một nhánh mới và chuyển đến nhánh đó nếu nó không tồn tại
- git checkout -b NewBranch

12. Merge Branches

- git merge NameBranch
