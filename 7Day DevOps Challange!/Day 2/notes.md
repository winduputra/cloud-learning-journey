# 📅 Day 2 – Setting Up AWS EC2 & Remote Development Environment

## ✅ Key Learning Today:
Hari ini saya mempelajari **cara membangun environment pengembangan aplikasi web secara remote menggunakan AWS EC2 dan VS Code**.
Ini adalah pondasi awal untuk membangun pipeline DevOps di hari-hari berikutnya.

## 🛠️ Tools & Technology Used:
- **AWS EC2** (Amazon Linux 2)
- **IAM User** for secure access
- **VS Code** + **Remote SSH Extension**
- **Apache Maven** & **Amazon Corretto 8 (Java 8)**

## 🔍 Step-by-Step Summary

### 1. ✅ Setup IAM User
- Membuat IAM User khusus untuk mengakses AWS CLI & EC2 dengan permission terbatas.
- Men-generate **Access Key ID** dan **Secret Access Key**.
- Konfigurasi AWS CLI:
   ```bash
   aws configure
   ```

### 2. ✅ Launch EC2 Instance
- Memilih **Amazon Linux 2 AMI**
- Instance type: `t2.micro`
- Membuka port **22 (SSH)** dan port **8080 (untuk web app nanti)** di Security Group.
- Mendownload key-pair `.pem` untuk akses SSH.

### 3. ✅ Install & Setup VS Code
- Install **Visual Studio Code**
- Tambahkan extension **Remote - SSH**
- Menambahkan konfigurasi SSH di `~/.ssh/config` supaya koneksi lebih mudah.

### 4. ✅ Remote SSH to EC2
- Tes koneksi SSH:
   ```bash
   ssh -i "my-key.pem" ec2-user@<EC2-PUBLIC-IP>
   ```
- Berhasil masuk ke server EC2 melalui terminal di VS Code.

### 5. ✅ Install Apache Maven & Amazon Corretto 8
- Update package manager:
   ```bash
   sudo yum update -y
   ```
- Install Java (Corretto 8):
   ```bash
   sudo amazon-linux-extras enable corretto8
   sudo yum install java-1.8.0-amazon-corretto -y
   ```
- Install Maven:
   ```bash
   sudo yum install maven -y
   ```

### 6. ✅ Create a Simple Java Web App
- Generate template Maven project:
   ```bash
   mvn archetype:generate
   ```
- Edit kode secara manual menggunakan `vim` / `nano`.

### 7. ✅ Connect EC2 Instance with VS Code
- Buka file project secara remote dan edit lebih nyaman via VS Code.
- Belajar perbedaan **edit manual (CLI)** dan **pakai IDE.**

## 🎯 What I Learned Today
- Cara provisioning EC2 instance.
- Konsep **remote development** menggunakan SSH.
- Pentingnya automation dan tools untuk mempermudah workflow DevOps.
- Dasar-dasar struktur project Maven dan Java environment.

## 🔜 Next Step (Day 3 Preview):
- Mulai menyiapkan **CI/CD pipeline** untuk otomatisasi build & deployment.
- Kemungkinan akan menggunakan **GitHub Actions** atau **Jenkins**.

> ✅ Repo ini adalah dokumentasi perjalanan belajar saya sebagai transisi dari SysAdmin ke Cloud & DevOps Engineer.
> Semua feedback dan saran sangat saya terima. 🙏
