# 🔧 Course Setup Guide  
### Scientific Programming with Python 🐍

Welcome! This guide will help you install Python, set up Git & GitHub, and learn how to submit homework using **GitHub Classroom**.  

---

## 🐍 1. Install Python

- Download from [python.org/downloads](https://www.python.org/downloads/)  
- Install **Python 3.11+**  
- On Windows → ✅ check *“Add Python to PATH”* during install  

**macOS (with Homebrew):**
```bash
brew install python
```

**Ubuntu/Debian:**
```bash
sudo apt update
sudo apt install python3 python3-pip -y
```

---

## ✅ 2. Verify Installation
```bash
python --version
```
Expected output:
```
Python 3.x.x
```

> ⚠️ On Linux/macOS, use `python3` and `pip3`.  
> On Windows, use `python` and `pip`.

---

## 📂 3. Virtual Environments (Optional, Advanced)

Keep project dependencies isolated:

```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.venv\Scripts\activate      # Windows
```

Deactivate with:
```bash
deactivate
```

---

## 📦 4. Install Dependencies

Use `pip` to add packages:
```bash
pip install pytest
```

Or install everything from `requirements.txt`:
```bash
pip install -r requirements.txt
```

---

## 🐙 5. Install Git

- Download from [git-scm.com/downloads](https://git-scm.com/downloads)  
- Verify installation:
```bash
git --version
```

Configure your identity:
```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

---

## 🚀 6. GitHub Setup

- Create an account at [github.com](https://github.com)  
- You’ll use GitHub to receive and submit homework via **GitHub Classroom**

---

## 🎓 7. GitHub Classroom Workflow

### 1️⃣ Accept the Assignment
- Open the **link** shared on Teams  
- GitHub will create a **private repo** for you in the course organization  
- Confirm the repo exists and is private  

### 2️⃣ Clone Your Repo
```bash
git clone <repo-url>
cd <repo-name>
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Work Locally
- Open the project in your editor  
- Implement solutions  
- Run tests to check:
```bash
pytest
# or run a specific test:
pytest tests/task_name.py
```

✅ Green tests → you’re ready to submit  
❌ Red tests → fix errors before committing  

### 5️⃣ Stage & Commit
```bash
git add .
git commit -m "HW0: implemented"
```

### 6️⃣ Push to GitHub
```bash
git push
```

### 7️⃣ Verify Submission
- Go to your repo on GitHub  
- Open the **Pull Requests (PR)** tab  
- Check feedback from the autograder:  
  - ✅ Green → submission successful  
  - ❌ Red → fix code, commit, and push again  

---

## 🧭 Cheat Sheets

### Python
- Run script: `python file.py`  
- REPL: `python`  
- Install package: `pip install <name>`  
- Virtual env: `python -m venv .venv`  

### Git
- Clone: `git clone <url>`  
- Status: `git status`  
- Stage: `git add <file>` / `git add .`  
- Commit: `git commit -m "message"`  
- Push/Pull: `git push` / `git pull`  
- History: `git log`  

---

## 🎉 You’re All Set!
- ✅ Python installed & working  
- ✅ Git & GitHub configured  
- ✅ GitHub Classroom workflow clear  

You’re ready to start coding and submit your assignments 🚀
