# Git_detector
# 🔍 Git Detector

A Python-based tool designed to scan Git repositories for potential sensitive data leaks, such as API keys, passwords, private keys, and certificates. It analyzes the entire Git history, ensuring no hidden secrets escape detection.

---

## 🚀 Features
- **Deep Scan:** Traverses full Git commit history.
- **Sensitive Data Detection:** Identifies:
  - 🔑 Passwords
  - 🗝️ API Keys (AWS, OpenAI, Google, etc.)
  - 📄 RSA & SSH Private Keys
  - 🔐 TLS/SSL Certificates
  - 🗃️ Database Credentials
- **User-Friendly Output:** Color-coded results for easy analysis.

---

## 📦 Requirements
Before running the tool, install the necessary dependencies:

```bash
pip install -r requirements.txt
