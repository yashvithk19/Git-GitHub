# Learn Git & GitHub from Scratch

## Introduction
This repository serves as a beginner-friendly guide to learning Git and GitHub from scratch. Follow the steps below to install Git, configure it, and use it to manage your projects with GitHub.

---

## 1️⃣ Installing Git
### Windows:
1. Download Git from [git-scm.com](https://git-scm.com/downloads).
2. Run the installer and select the default options (except for the PATH option; choose **"Git from the command line and also from 3rd-party software"**).
3. Restart your computer.
4. Verify the installation:
   ```sh
   git --version
   ```

### macOS:
1. Install Git using Homebrew:
   ```sh
   brew install git
   ```
2. Verify the installation:
   ```sh
   git --version
   ```

### Linux (Ubuntu/Debian):
1. Install Git via terminal:
   ```sh
   sudo apt update
   sudo apt install git
   ```
2. Verify the installation:
   ```sh
   git --version
   ```

---

## 2️⃣ Configuring Git
Once Git is installed, configure your username and email:
```sh
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```
To check your configuration:
```sh
git config --list
```

---

## 3️⃣ Initializing a Git Repository
1. Open a terminal and navigate to your project folder:
   ```sh
   cd path/to/your/folder
   ```
2. Initialize Git:
   ```sh
   git init
   ```
3. Add files to Git:
   ```sh
   git add .
   ```
4. Commit the changes:
   ```sh
   git commit -m "Initial commit"
   ```

---

## 4️⃣ Connecting to GitHub
1. Create a **new repository** on GitHub.
2. Copy the repository URL.
3. Link your local Git repository to GitHub:
   ```sh
   git remote add origin https://github.com/your-username/repository-name.git
   ```
4. Push the code to GitHub:
   ```sh
   git branch -M main
   git push -u origin main
   ```

---

## 5️⃣ Common Git Commands
### Checking Status
```sh
git status
```

### Viewing Commit History
```sh
git log --oneline
```

### Creating a New Branch
```sh
git checkout -b new-branch-name
```

### Switching Branches
```sh
git checkout branch-name
```

### Merging Branches
```sh
git merge branch-name
```

### Pulling Latest Changes from GitHub
```sh
git pull origin main
```

### Cloning a Repository
```sh
git clone https://github.com/username/repository-name.git
```

---

## 6️⃣ Undoing Changes
### Undo Last Commit (Keep Changes)
```sh
git reset --soft HEAD~1
```

### Undo Last Commit (Discard Changes)
```sh
git reset --hard HEAD~1
```

### Remove a File from Git Tracking
```sh
git rm --cached filename
```

---

## 7️⃣ Working with GitHub
### Creating a Pull Request
1. Push your changes to a **new branch**.
2. Go to GitHub and navigate to your repository.
3. Click on **Compare & Pull Request**.
4. Add a description and click **Create Pull Request**.

### Forking a Repository
1. Open a repository on GitHub.
2. Click the **Fork** button.
3. Clone your forked repository:
   ```sh
   git clone https://github.com/your-username/forked-repository.git
   ```

---

## 8️⃣ Troubleshooting
### Check Remote Repository URL
```sh
git remote -v
```

### Fix "fatal: remote origin already exists"
```sh
git remote remove origin
```
Then, re-add the correct remote:
```sh
git remote add origin https://github.com/your-username/repository-name.git
```

### Fix "Permission Denied (Publickey)" Error
- Generate a new SSH key:
  ```sh
  ssh-keygen -t rsa -b 4096 -C "your-email@example.com"
  ```
- Add the SSH key to GitHub under **Settings → SSH and GPG Keys**.

---

If you found this guide helpful, don't forget to ⭐ this repository! 😊
