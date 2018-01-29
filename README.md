# GitHub
![octocat.png](https://raw.githubusercontent.com/LITTL3BEAR/foo/master/octocat.png)

## Info
Git cheat sheet (PDF) : https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf

Git cheat sheet : https://services.github.com/on-demand/downloads/github-git-cheat-sheet/

สอบ : github วิธีแก้ conflict

## Setup
$ git config --global user.name "your name"

$ git config --global user.email "your email"

$ git config --list // แสดง config

## Create
$ git init // สร้าง .git และ repo เปล่า

$ git status // แสดงสถานะ

$ git echo "your message" >> {your file} // สร้างไฟล์

$ git add {your file}

$ git add . // เพิ่มทั้งหมด

$ git add '*.txt' // เพิ่มแฉพาะสกุลไฟล์

$ git commit -m "your message"

$ git log // แสดงการทำงาน

$ git log --oneline // แสดงการทำงานแบบย่อ

$ git log --oneline --decorate --

## Reset
$ git checkout {file name} // กู้คืนไฟล์

$ git reset {file name} // กู้คืนไฟล์ หลัง add

$ git reset --soft HEAD~1 // กู้คืนไฟล์ หลัง commit

??? git reset --soft "HEAD^"

??? git reset --soft {file name} 

## Branch
$ git branch // ดู branch

$ git branch -a // ดู branch ทั้งหมด

$ git branch {branch name} // สร้าง branch

$ git checkout {branch name} // สลับ branch

$ git checkout -b {branch name} // สร้างและสลับ branch

$ git push -u origin {branch name} // อัพ branch ขึ้น server

$ git merge {branch name} // รวม bracnh กับ master *(ทำใน master)

$ git checkout {branch name} {file name} // ย้ายไฟล์จาก branch ต้นทาง **(สลับมาอยู่ใน branch ปลายทางก่อน)

$ git branch -d {branch name} // ลบ branch

$ git push origin --delete {branch name} // ลบ branch ใน remote

$ git merge --no-ff {branch name} // รวมไฟล์จาก branch

## Repo
$ git remote add origin {your repo url} // remote ไปยัง repo ที่สร้าง

$ git remote -v // ตรวจสอบการ remote

$ git push -u origin master // การส่งถึง github ครั้งแรก

## Tag
$ git tag {tag name} // การอ้างอิง

$ git push --tags

$ git checkout {tag name} // ย้ายไปยังที่อ้างอิง

$ git tag -d {tag name} // ลบ tag

$ git push origin --delete {tag name} // ลบ tag ใน remote

## Other
$ git fetch // เปรียบเทียบ

$ git merge origin/master // อัพเดท

$ git pull // การ fetch+merge

$ git push // ส่งขึ้น server

$ git clone {git url}

$ git remote add upstream {git url}

$ git fetch upstream

$ git merge upstream/master

$ git more {file name} // แสดงรายละเอียดไฟล์

$ git rm {file name} // ลบไฟล์

??? git stash

??? git stash pop

## Logout
$ git config --global --unset user.name

$ git config --global --unset user.email
