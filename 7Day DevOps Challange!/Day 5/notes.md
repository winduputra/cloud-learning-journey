# 📅 Day 5 - Continuous Integration with AWS CodeBuild

## ✅ Key Learnings Today:

Today I learned how to implement **Continuous Integration (CI)** using **AWS CodeBuild** to automate the build process of my web app.

---

## 🛠️ Tools & Services Used:
- **AWS CodeBuild**
- **GitHub**
- **Amazon S3**
- **AWS CodeArtifact**
- **IAM Roles & Policies**

---

## 🔍 Step-by-Step Summary

### 1. ⚙️ Setup CodeBuild Project
- Create a CodeBuild project and connect it with my GitHub repository.

### 📝 Define buildspec.yml
- Create a `buildspec.yml` file to automatically define the build steps.

### 📦 Store Artifacts in S3
- Save the build artifacts to an Amazon S3 bucket for future deployment.

### 4. 🔑 Update IAM Role
- Give CodeBuild's IAM Role permission to access the CodeArtifact repository.

### 5. 🛠️ Troubleshoot Build Errors
- Resolve common errors, such as credentials, missing dependencies, or syntax errors in `buildspec.yml`.

### 💎 Beyond Build: Automated Testing
- Adds a step to run automated tests (if any) as part of the build process.


---

## 🎯 What I Learned Today

- What is CI and why is it important in DevOps pipeline.
- How to use CodeBuild for automated builds from GitHub repos.
- Managing artifacts and IAM access properly.
- Setting up a stable and scalable build process for testing.

---

> This was an important step in my journey from SysAdmin to Cloud & DevOps Engineer.
