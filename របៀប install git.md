ការដំឡើង **Git** អាចធ្វើបានងាយៗ តាមជំហានខាងក្រោម។ Git គឺជា **version control system** ដែល developer ប្រើដើម្បីគ្រប់គ្រង code និងធ្វើការជាមួយ **GitHub** ឬ **GitLab**។

---

## 1️⃣ Install Git នៅលើ **Windows**

1. ចូលទៅកាន់ Website ផ្លូវការ
   👉 [https://git-scm.com/](https://git-scm.com/)

2. ចុច **Download for Windows**

3. បន្ទាប់ពី Download រួច

   * បើក File `.exe`
   * ចុច **Next** ទៅរហូត
   * ចុច **Install**

4. ពេល Install រួច ចុច **Finish**

5. តេស្តថា Git ដំណើរការ
   បើក **Command Prompt** ឬ **Terminal** ហើយវាយ៖

```bash
git --version
```

បើបង្ហាញ version មានន័យថា Install បានជោគជ័យ។

---

## 2️⃣ Install Git នៅលើ **Mac**

បើអ្នកប្រើ Mac អាច Install តាម **Terminal**

```bash
brew install git
```

ឬ

```bash
git --version
```

Mac នឹងសួរ install **Command Line Tools** ហើយ install អោយដោយស្វ័យប្រវត្តិ។

---

## 3️⃣ កំណត់ Git Username និង Email (សំខាន់)

បន្ទាប់ពី install ត្រូវ config ម្តង៖

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

ឧទាហរណ៍

```bash
git config --global user.name "Chantha"
git config --global user.email "chantha@gmail.com"
```

---

✅ **ពិនិត្យ Config**

```bash
git config --list
```

---

💡 **Git ប្រើសម្រាប់**

* Save history code
* Collaborate ជាមួយ team
* Upload project ទៅ **GitHub**

---

✅ បើអ្នកចង់ ខ្ញុំអាចបង្ហាញបន្ត៖

* របៀប **Connect Git ជាមួយ GitHub**
* របៀប **push project ទៅ GitHub step by step**
* **Basic Git commands (10 command សំខាន់)** 🚀
