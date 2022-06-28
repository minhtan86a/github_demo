# Setup name and email
- git config --global user.name "TanNguyen" (create username)
- git config --global user.email "minhtan86a@gmail.com" (create email)
- git config --global user.name (check username)
- git config --global user.email (check email)


# Terms
- Repository (Repo)
- Branch (default: master) (1 project có thể có nhiều branch)
- Conflict (xung đột, nếu có xung đột khi 2 branch sửa code trên cùng 1 file thì phải kiểm tra lại xem giữ cái nào rồi add và commit mới merge được, commit ko cần ghi chú vì đang giải quyết 1 conflict)
- Local (trên máy tính)
- Remote (trên server)

# Commands
- git init (Chuyển project thành 1 repository)
- git status (thấy được toàn bộ files trong project)
- git add {file name}(chuẩn bị lưu lại thời điểm của project)
- git add . (lưu all files)
- git reset (bỏ các file đã lưu)
- git commit -m 'write something' (chính thức lưu để up lên repo | -m là message "initial commit" )
- git log (xem thời điểm lưu)
- git log --oneline

# Branch and Merge
- git branch (list all branchs)
- git branch -d [branch-name] (xóa 1 branch)
- git branch [branch-name] (create a new branch at the current commit)

- git checkout -b [branch-name] (Create and check out a new branch named [branch] | Drop the -b flag to checkout an existing branch | ex: git checkout -b dev | Switched to a new branch)
- git checkout [id] (trở lại 1 thời điểm theo id cụ thể | use git log to get id | ex: id = id của commit)
- git checkout [branch-name] (switch to another branch and check it out into your working directory, ex: git checkout master)

- git merge [branch-name] (Merge [branch-name] into the current branch)

# Share and Update
- git remote add [alias] [url] ( create 1 alias cho link remote | [alias] is origin | ex: git remote add origin https://github.com/minhtan86a/github_demo.git
- git push [alias] [branch] ( upload project from local len remote | ex: -git push origin master )
- git push [repo-url] [branch-name] (upload project from local len remote)

# REMOTE REPOSITORIES
- git clone [repo-url] (retrieve an entire repository from a hosted location via URL | nếu tải project từ server thì use "-git push" để tải code lên server)
- git push [alias] [branch] | git push (ex: git push -u origin dev | origin: [alias] of remote server, dev: [branch-name] | upload 1 branch từ local lên remote server)
- git fetch [alias] (fetch down all the branches from that Git remote | ex: git fetch origin | origin: [alias] of remote server | tải branchs trên remote về)

- sử dụng Pull request tren github để merge 1 branch mới vào master
- git pull [url](tải về thay đổi trên github)
- Fork dùng để chỉnh sửa code của 1 ai đó trên github sau đó tạo 1 pull request để xin tác giả thêm vào và chờ duyệt.