# DEV

## Branch
$ git branch // ดู branch

$ git branch -a // ดู branch ทั้งหมด

$ git branch {branch name} // สร้าง branch

$ git checkout {branch name} // สลับ branch

$ git checkout -b {branch name} // สร้างและสลับ branch

$ git push origin {branch name} // อัพ branch ขึ้น server

$ git merge {branch name} // รวม bracnh กับ master *(ทำใน master)

$ git checkout {branch name} {file name} // ย้ายไฟล์จาก branch ต้นทาง **(สลับมาอยู่ใน branch ปลายทางก่อน)

$ git branch -d {branch name} // ลบ branch

$ git merge --no-ff {branch name} // รวมไฟล์จาก branch
