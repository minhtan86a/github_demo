# Setup name and email
git config --global user.name "TanNguyen"
git config --global user.email "minhtan86a@gmail.com"

# Check name and email
- git config --global user.name
- git config --global user.email


# Terms

- Repository (Repo)
- Branch (default: master) (1 project có thể có nhiều branch)

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
- git checkout <branchname> (trở lại hiện tại, ex: git checkout master)
- git branch
- git checkout -b <branchname> (tạo branch mới, ex: git checkout -b dev)