# Git & Github

### Introduction to Git
- **Git** is a distributed version control system that tracks changes in source code during software development.
- It allows multiple developers to work on a project simultaneously without interfering with each other's work.

### Setting Up Git
1. **Installation**:
   - Check if Git is installed: `git --version`
   - Install Git on Linux:
     - Ubuntu/Debian: `sudo apt update && sudo apt install git -y`
     - Fedora: `sudo dnf install git -y`
     - CentOS: `sudo yum install git -y`
     - Arch Linux: `sudo pacman -S git`
2. **Configuration**:
   - Set your name: `git config --global user.name "Your Name"`
   - Set your email: `git config --global user.email "[email protected]"`
   - Verify configuration: `git config --list`

### Basic Git Commands
- Initialize a repository: `git init`
- Clone a repository: `git clone <repository-url>`
- add repo https: `git remote add origin <repo address>`
- Check status: `git status`
- Add files to staging: `git add <file-name>` or `git add .`
- Commit changes: `git commit -m "Commit message"`
- push code : `git push -u origin <branch-name>`
- View commit history: `git log` or `git log --oneline`

### Branching and Merging
- Create a new branch: `git branch <branch-name>`
- Switch to a branch: `git checkout <branch-name>` or `git switch <branch-name>`
- Rename branch : `git branch -m <branch-name` 
- Merge branches: `git merge <branch-name>`
- Delete a branch: `git branch -d <branch-name>`

### Working with Remote Repositories
- Add a remote repository: `git remote add origin <repository-url>`
- Push changes: `git push origin <branch-name>`
- Pull changes: `git pull origin <branch-name>`
- Clone a repository: `git clone <repository-url>`

### SSH Authentication
1. **Generate SSH Key**:
   - `ssh-keygen -t rsa -b 4096 -C "[email protected]"`
2. **Add SSH Key to Agent**:
   - Start agent: `eval "$(ssh-agent -s)"`
   - Add key: `ssh-add ~/.ssh/id_rsa`
3. **Add SSH Key to GitHub**:
   - Copy key: `cat ~/.ssh/id_rsa.pub`
   - Add to GitHub under SSH keys settings.
4. **Test SSH Connection**:
   - `ssh -T [email protected]`

### Best Practices
- Write clear and descriptive commit messages.
- Use branches to manage new features and bug fixes.
- Regularly pull changes from the remote repository to stay updated.
- Review code changes before merging to the main branch.

#### **@author**: Ripan Baidya 
---

