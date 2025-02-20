# 🔒 Security Testing Repository

This repository contains **intentionally vulnerable code** for security analysis and testing.  
It includes **GitHub Actions workflows** that automatically scan the code for security vulnerabilities  
using **Cppcheck** (for C/C++) and **Semgrep** (for multiple languages).  

---

## 🚀 Features
- 🛠 **Vulnerable Code** – Contains code with security flaws for testing.
- 🤖 **Automated Security Scans** – Runs **Cppcheck** and **Semgrep** on code changes.
- 📊 **GitHub Security Dashboard Integration** – Reports are uploaded to GitHub’s security panel.
- 📂 **SARIF Report Uploads** – Allows reviewing scan results directly in GitHub.

---
## 📁 Repository Structure
📦 security-testing-repo ├── .github/workflows/ # GitHub Actions workflows │ ├── cppcheck.yml # Cppcheck security scan │ ├── semgrep.yml # Semgrep security scan ├── vulnerable-source-code/ # Directory with intentionally vulnerable code │ ├── test.c # Example vulnerable C code │ ├── test.cpp # Example vulnerable C++ code ├── README.md # This file

markdown
Copy
Edit

---

## ⚡ GitHub Actions Workflows

### 🔹 **Cppcheck (C/C++ Security Scan)**
- **Runs on:** `push` to `master`
- **Scans:** `vulnerable-source-code/`
- **Uploads:** SARIF results to the **GitHub Security Dashboard**.

#### **Workflow Location:**
📄 `.github/workflows/cppcheck.yml`

### 🔹 **Semgrep (Static Code Analysis)**
- **Runs on:** `push`, `pull_request`
- **Scans:** `vulnerable-source-code/`
- **Uploads:** SARIF reports for **GitHub Code Scanning Alerts**.

#### **Workflow Location:**
📄 `.github/workflows/semgrep.yml`

---

## 📊 Viewing Security Reports
1. Go to **GitHub → Security Tab → Code Scanning Alerts**.
2. View **Cppcheck and Semgrep scan results**.
3. Click on **SARIF reports** for detailed analysis.
