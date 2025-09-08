## 🚀 Git Command Reference

### 1. 🔧 Setup & Configuration
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
git init
```

### 2. 📦 Repository Basics
```bash
git clone <repo-url>
git status
git add <file-name>         # or use . to add all
git commit -m "Your message"
git push origin main
git pull origin main
```

### 3. 🌿 Branching & Merging
```bash
git branch                   # list branches
git branch <branch-name>     # create new branch
git checkout <branch-name>   # switch branch
git checkout -b <branch-name> # create + switch
git merge <branch-name>      # merge into current branch
```

### 4. 🧹 Undo & Reset
```bash
git reset <file>             # unstage file
git reset --hard HEAD        # discard all local changes
git checkout -- <file>       # discard changes in file
git revert <commit-id>       # undo a commit safely
```

### 📜5.  Log & History
```bash
git log                      # view commit history
git log --oneline --graph    # compact visual history
git show <commit-id>         # details of a commit
```

### 🔄6.  Sync & Rebase
```bash
git fetch                    # fetch latest changes
git pull --rebase origin main
git push --force origin main # use with caution
```

### 🧪7.  Stashing Work
```bash
git stash                    # save changes temporarily
git stash apply              # reapply stashed changes
git stash list               # view stashes
```

### 🔍8.  Remote & Tracking
```bash
git remote -v                # view remote URLs
git remote add origin <url> # add remote
git branch -vv               # track remote branches
```
### 9. Push new project on github
## 🚀 Steps to Push Local Project to GitHub

1. **Initialize Git in your local project folder**
   ```bash
   git init
   ```

2. **Rename the default branch to `main` (recommended for modern GitHub workflows)**
   ```bash
   git branch -M main   # Renames current branch to 'main'
   ```

3. **Add all files to staging**
   ```bash
   git add .
   ```

4. **Commit your changes**
   ```bash
   git commit -m "Initial commit"
   ```

5. **Create a new repository on GitHub**  
   Go to [GitHub](https://github.com) → Click **New Repository** → Name it → Click **Create Repository**

6. **Link your local project to the GitHub repo**
   ```bash
   git remote add origin https://github.com/your-username/your-repo-name.git
   ```

7. **Push your code to GitHub**
   ```bash
   git push -u origin main
   ```

> ⚠️ If your GitHub repo already has commits (like a README), run:
```bash
git pull --rebase origin main
git push origin main
```

8. **Verify your code is live on GitHub**  
   Go to your GitHub repo and refresh the page.
---

## 10. **Change remote and push code to remote**
See current remotes and URLs
 ```bash
git remote -v
 ```

(Optional) list remote branches
 ```bash
git fetch --all
git branch -r
 ```

Replace the old origin URL with the new repo URL

 ```bash
git remote set-url origin https://github.com/ankitsharma2002/PlayWrightAutomationFramework_Project.git
 ```

Alternative: remove and re-add origin
 ```bash
git remote remove origin
git remote add origin https://github.com/ankitsharma2002/PlayWrightAutomationFramework_Project.git
 ```

Verify the change
 ```bash
git remote -v
 ```

### create a new repository on the command line

echo "# JBDL_mini_project" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ankitsharma2002/JBDL_mini_project.git
git push -u origin main

### push an existing repository from the command line

git remote add origin https://github.com/ankitsharma2002/JBDL_mini_project.git
git branch -M main
git push -u origin main
