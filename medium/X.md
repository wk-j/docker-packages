Build และ Publish Docker (Image) ด้วย GitHub Actions

1. สร้าง Project ด้วย .NET CLI ตั้งชื่อว่า `MyWeb`

dotnet new webapi  --language C# --output src/MyWeb

2. เขียน `Dockerfile`

3. เพิ่ม Config สำหรับ GitHub Actions ใต้โฟลเดอร์ workflow `.github/workflows/build-tag.yml`

- :Account ชื่อ Account GitHub
- :Repository ชื่อ Project ใน GitHub
- :ImageName ชื่อ Image

3. Commit โค้ด

```bash
git commit -m "Initial commit"
git push origin master

git tag v0.1
git push origin v0.1
```
