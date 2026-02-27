

---

# 📘 របៀបដំឡើង VS Code

## 💻 សម្រាប់ Windows

1. ចូលទៅកាន់គេហទំព័រផ្លូវការ៖
   👉 [https://code.visualstudio.com/](https://code.visualstudio.com/)

2. ចុច **Download for Windows**

3. បើកឯកសារ `.exe` ដែលបានទាញយក

4. អនុវត្តតាមជំហានដំឡើង:

   * ✔️ Accept agreement
   * ✔️ ជ្រើសទីតាំងដំឡើង
   * ✔️ គូសធីក **Add to PATH** (សំខាន់)
   * ✔️ គូសធីក **Create Desktop Icon**

5. ចុច **Install**

6. ចុច **Finish** ហើយបើក VS Code

---

## 🍎 សម្រាប់ macOS

1. ចូលទៅ [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. ចុច **Download for Mac**
3. បើកឯកសារ `.zip`
4. អូស **Visual Studio Code** ទៅក្នុង **Applications**
5. បើកកម្មវិធី

👉 បើចង់ប្រើ `code` command ក្នុង Terminal:

* បើក VS Code
* ចុច `Cmd + Shift + P`
* វាយ `Shell Command: Install 'code' command in PATH`
* ចុច Enter

---

## 🐧 សម្រាប់ Linux (Ubuntu/Debian)

### វិធីទី 1: ប្រើ .deb

```bash
sudo apt install ./code_*.deb
```

### វិធីទី 2: ប្រើ Snap

```bash
sudo snap install --classic code
```

---

## ✅ ពិនិត្យថាដំឡើងបានជោគជ័យ

បើក Command Prompt ឬ Terminal ហើយវាយ៖

```bash
code --version
```

បើបង្ហាញលេខ version មានន័យថាដំឡើងបានជោគជ័យ 🎉

---

## 🚀 Extension ដែលគួរតែដំឡើង

ចុច `Ctrl + Shift + X` ដើម្បីបើក Extensions ហើយដំឡើង៖

* ESLint
* Prettier
* Live Server
* GitLens
* PHP Intelephense (សម្រាប់ Laravel)
* Tailwind CSS IntelliSense

---

## 🔥 បើក Project

ចូលទៅ Folder Project ហើយវាយ៖

```bash
code .
```

វានឹងបើក folder នោះក្នុង VS Code។

