# 📅 Day 4 – Secure Packages with AWS CodeArtifact

## ✅ Key Learning Today:

Hari ini saya mempelajari cara menggunakan **AWS CodeArtifact** sebagai repositori Maven pribadi untuk mengelola dependencies pada aplikasi web.  
Langkah ini penting dalam proses DevOps untuk memastikan dependencies aman dan terkendali.

## 🛠️ Tools & Technology Used:
- **AWS CodeArtifact**
- **IAM Roles & Policies**
- **Maven**
- **AWS EC2 (as app environment)**

## 🔍 Step-by-Step Summary

### 1. 🗂️ Set Up CodeArtifact
- Membuat domain dan repository di AWS CodeArtifact.
- Konfigurasi repo sebagai Maven repository privat.

### 2. 🛡️ Configure IAM Access from EC2
- Membuat IAM Role dengan permission ke CodeArtifact.
- Attach role tersebut ke EC2 instance.
- Konfigurasi CLI agar EC2 bisa authenticate ke CodeArtifact.

### 3. ✅ Verify Maven Connection
- Konfigurasi `.m2/settings.xml` untuk menunjuk ke repository CodeArtifact.
- Jalankan build project → Maven berhasil mengunduh dependencies dari CodeArtifact.

### 4. 💎 Add Custom Package
- Membuat custom package Java.
- Upload ke repository CodeArtifact via Maven deploy plugin.

## 🎯 What I Learned Today
- Cara menyimpan dan mengatur dependencies secara privat menggunakan CodeArtifact.
- Pentingnya integrasi IAM untuk akses antar layanan AWS.
- Menghubungkan Maven ke repository privat dan deploy package secara aman.

## 🔜 Next Step (Day 5 Preview):
- Mulai membuat pipeline otomatisasi CI/CD dengan GitHub Actions.

> ✅ Ini adalah bagian dari transisi saya dari SysAdmin ke DevOps/Cloud Engineer.
> Semua feedback dan masukan sangat diterima 🙏
