# 📅 Day 3 – Setting Up GitHub Repository and Source Control Basics

## ✅ Key Learning Today:

Hari ini saya mempelajari **cara membuat repository GitHub dan mengelola source code secara version control**.  
Ini adalah langkah penting untuk menyimpan source code web app Java saya dan menyiapkan kolaborasi tim di masa depan.

## 🛠️ Tools & Technology Used:
- **GitHub**
- **Git CLI**
- **AWS EC2 (as the development environment)**

## 🔍 Step-by-Step Summary

### 1. ✅ Set up a GitHub Repository
- Membuat repository baru di GitHub untuk menyimpan source code Java web app.
- Repository bersifat **private** untuk menjaga keamanan source code.

### 2. ✅ Configure Git & Local Repository
- Konfigurasi user:
   ```bash
   git config --global user.name "winduputra"
   git config --global user.email "windups21@gmail.com"
   ```
- Inisialisasi Git:
   ```bash
   git init
   git remote add origin https://github.com/username/repo-name.git
   ```

### 3. ✅ First Commit & Push
- Menambahkan semua file dan membuat commit pertama:
   ```bash
   git add .
   git commit -m "Initial commit"
   git push -u origin master
   ```

### 4. ✅ Setup README File
- Menambahkan **README.md** untuk memperkenalkan project kepada user yang membuka repository.

## 🎯 What I Learned Today
- Dasar-dasar version control dengan Git.
- Workflow push dan pull antara local repo & GitHub.
- Pentingnya dokumentasi project dengan README.md.

## 🔜 Next Step (Day 4 Preview):
- Belajar tentang **AWS CodeArtifact** untuk menyimpan dependencies (library/package) yang dibutuhkan oleh web app.

> ✅ Repo ini adalah dokumentasi perjalanan belajar saya sebagai transisi dari SysAdmin ke Cloud & DevOps Engineer.
> Feedback dan saran sangat saya terima. 🙏
