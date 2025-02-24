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
```

---

## ⚡ Pre-execution Setup
Before running the tool, ensure all Git repositories are marked as trusted to avoid permission errors:

```bash
git config --global --add safe.directory '*'
```

---

## 💻 Usage

1. **Clone the repository:**

   ```bash
   git clone <your-repo-link>
   cd Git_detector
   ```

2. **Run the tool:**

   ```bash
   python git_detector.py
   ```

3. **For scanning a specific repository:**

   ```bash
   python git_detector.py /path/to/repository
   ```

---

## 📝 Output Example

The tool highlights sensitive data types along with their respective commit IDs for easy tracking and removal.

```
[Password] Hardcoded password found
Commit: cc8a4c6
Key: my_secret_password

[RSA Private Key] RSA Private Key found
Commit: b20f5b8
Key: -----BEGIN RSA PRIVATE KEY-----
```

---

## ⚖️ Disclaimer
This tool is intended for ethical use only. Always ensure you have proper authorization before scanning repositories.

---

---

## Contribution
This repo is open for contribution, need to update regex patterns for different keys (APIs keys, passwords, usernames, certificate keys). If you'd like to improve **Git_detector**, check out the [Contributing Guidelines](CONTRIBUTING.md) and open a pull request.

---

🚀 **Happy Hunting!**
