# Setup name and email
git config --global user.name "TanNguyen"
git config --global user.email "minhtan86a@gmail.com"

# Check name and email
- git config --global user.name
- git config --global user.email


# Terms

- Repository (Repo)
- Branch (default: master) (1 project có thể có nhiều branch)
- Conflict (xung đột, nếu có xung đột khi 2 branch sửa code trên cùng 1 file thì phải kiểm tra lại xem giữ cái nào rồi add và commit mới merge được, commit ko cần ghi chú vì đang giải quyết 1 conflict)
- Local (trên máy tính)
- Remote (trên server)

# Commands

- git init (Chuyển project thành 1 repository)
- git status (thấy được toàn bộ files trong project)
- git add <file name>(chuẩn bị lưu lại thời điểm của project)
- git add . (lưu all files)
- git reset (bỏ các file đã lưu)
- git commit -m 'write something' (chính thức lưu để up lên repo, -m là message "initial commit" )
- git log (xem thời điểm lưu)
- git log --oneline
- git checkout <id> (trở lại 1 thời điểm ban đầu / cụ thể, ex: id = id của commit)
- git checkout <branch name> (trở lại 1 branch, ex: git checkout master)
- git checkout -b <branch name> (tạo branch mới, ex: git checkout -b dev)
- git merge <branch name> (tổng hợp lại các branch)
- git branch (list all branchs)
- git branch -d <branch name> (xóa 1 branch)
- git push <link repo của remote> <branch name>(upload project from local len remote)