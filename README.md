# 🐙 GitHub Cheat Sheet

เอกสารนี้รวบรวมคำสั่งพื้นฐานที่ใช้บ่อยใน GitHub เพื่อความสะดวกในการใช้งาน

---

## ⚙️ Git Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --list         # ดู config ทั้งหมด
```

---

## 📁 Initializing & Creating

```bash
git init                         # เริ่มต้น Git repo ใหม่
git status                       # ตรวจสอบสถานะไฟล์
echo "hello" >> file.txt         # สร้างไฟล์ใหม่
git add file.txt                 # เพิ่มไฟล์เข้า staging
git add .                        # เพิ่มไฟล์ทั้งหมด
git add '*.txt'                  # เพิ่มเฉพาะไฟล์ .txt
git commit -m "Your message"     # Commit
git log                          # ดูประวัติ
git log --oneline                # ดูประวัติแบบย่อ
```

---

## ♻️ Reset & Undo

```bash
git checkout file.txt            # ยกเลิกการแก้ไขไฟล์
git reset file.txt               # เอาไฟล์ออกจาก staging
git reset --soft HEAD~1          # Undo commit ล่าสุด (แต่ไม่ลบไฟล์)
# git reset --soft HEAD^         # เหมือน HEAD~1
```

---

## 🌿 Branching

```bash
git branch                       # ดู branch ปัจจุบัน
git branch -a                    # ดูทุก branch (local + remote)
git branch feature-x             # สร้าง branch ใหม่
git checkout feature-x           # สลับไป branch
git checkout -b feature-x        # สร้าง + สลับไป branch ใหม่
git merge --no-ff feature-x      # รวม branch โดยไม่ fast-forward
git branch -d feature-x          # ลบ branch local
git push origin --delete feature-x  # ลบ branch บน remote
```

> **Tip:**  
> ต้อง `checkout` มายัง branch ปลายทางก่อน หากจะดึงไฟล์จาก branch อื่น:

```bash
git checkout main                # อยู่ที่ main ก่อน
git checkout feature-x file.txt  # ดึงไฟล์จาก feature-x
```

---

## 🌐 Remote Repository

```bash
git remote add origin <url>      # เชื่อม repo กับ remote
git remote -v                    # ตรวจสอบ remote ที่เชื่อม
git push -u origin master        # Push ครั้งแรก
git push                         # Push ล่าสุด
git pull                         # ดึงข้อมูลจาก remote
git fetch                        # ดึงข้อมูลโดยไม่ merge
git merge origin/master          # merge หลัง fetch
git clone <url>                  # Clone repo
```

---

## 🏷️ Tagging

```bash
git tag v1.0.0                   # สร้าง tag
git push --tags                  # Push tag ขึ้น remote
git checkout v1.0.0              # Checkout ที่ tag
git tag -d v1.0.0                # ลบ tag ใน local
git push origin --delete v1.0.0  # ลบ tag บน remote
```

---

## 🧹 Stash (ซ่อนงานชั่วคราว)

```bash
git stash                        # เก็บงานที่ยังไม่ commit
git stash pop                    # ดึงงานล่าสุดกลับมา
```

---

## 🔧 File Management

```bash
git rm file.txt                  # ลบไฟล์และ stage deletion
git restore file.txt             # (Git 2.23+) กู้ไฟล์กลับ
```

---

## 🔓 Logout (ลบ config ส่วนตัว)

```bash
git config --global --unset user.name
git config --global --unset user.email
```

---
