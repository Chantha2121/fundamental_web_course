Here’s a clean **step-by-step document** you can follow (or share) for setting up SSH with GitHub.

---

# 📄 GitHub SSH Setup Guide (Windows / Git Bash)

## 🎯 Objective

Connect your local machine to GitHub using SSH so you can **clone, push, and pull without password**.

---

# 1️⃣ Check existing SSH keys

```bash
ls ~/.ssh
```

### ✅ If you see:

* `id_ed25519` and `id_ed25519.pub` → go to Step 3
* Nothing → go to Step 2

---

# 2️⃣ Generate a new SSH key

```bash
ssh-keygen -t ed25519 -C "your_email@gmail.com"
```

Press:

* Enter (save location)
* Enter (no passphrase)
* Enter (confirm)

---

# 3️⃣ Start SSH agent

```bash
eval "$(ssh-agent -s)"
```

Expected:

```bash
Agent pid XXXX
```

---

# 4️⃣ Add SSH key to agent

```bash
ssh-add ~/.ssh/id_ed25519
```

---

# 5️⃣ Verify key is added

```bash
ssh-add -l
```

Expected:

```bash
256 SHA256:XXXX your_email@gmail.com (ED25519)
```

---

# 6️⃣ Copy public key

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy everything (starts with `ssh-ed25519`)

---

# 7️⃣ Add SSH key to GitHub

Go to:
👉 [https://github.com/settings/keys](https://github.com/settings/keys)

Steps:

* Click **New SSH Key**
* Title: your PC name (e.g., "My Laptop")
* Paste your key
* Click **Add SSH Key**

---

# 8️⃣ Test SSH connection

```bash
ssh -T git@github.com
```

### ✅ Success:

```bash
Hi username! You've successfully authenticated...
```

---

# 9️⃣ Clone repository using SSH

```bash
git clone git@github.com:username/repository.git
```

---

# 🔁 Optional: Fix wrong remote URL

Check:

```bash
git remote -v
```

If HTTPS:

```bash
git remote set-url origin git@github.com:username/repository.git
```

---

# ⚠️ Common Errors & Fixes

## ❌ Permission denied (publickey)

✔ Run:

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

✔ Ensure key is added to GitHub

---

## ❌ Could not open a connection to your authentication agent

✔ Start agent:

```bash
eval "$(ssh-agent -s)"
```

---

## ❌ No such file

✔ Generate key again:

```bash
ssh-keygen -t ed25519 -C "your_email@gmail.com"
```

---

# 💡 Best Practice

* Always use **SSH** for development
* Avoid HTTPS (needs token every time)
* Keep your private key safe (`id_ed25519`)

---

# ✅ Final Checklist

✔ SSH key created
✔ SSH agent running
✔ Key added to agent
✔ Key added to GitHub
✔ SSH test success

---

If you want, I can convert this into:

* 📘 PDF
* 📊 Slide (PowerPoint)
* 🧾 Company SOP

Just tell me 👍
