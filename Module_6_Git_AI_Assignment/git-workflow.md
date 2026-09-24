# Git Version Control Workflow

## 1. Check Git Installation
```bash
git --version
```

## 2. Configure Git
```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

## 3. Initialize the Project
Open the project folder in VS Code terminal and run:
```bash
git init
```

## 4. Check Repository Status
```bash
git status
```

## 5. Add Files
```bash
git add .
```

## 6. Create the First Commit
```bash
git commit -m "Initial commit"
```

## 7. Connect GitHub Repository
After creating an empty repository on GitHub:
```bash
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/module-6-git-ai-assignment.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username.

## 8. Create a Feature Branch
```bash
git checkout -b feature/update-readme
```

## 9. Make a Change
Edit a file, save it, then run:
```bash
git add .
git commit -m "Update README"
```

## 10. Push the Branch
```bash
git push -u origin feature/update-readme
```

## 11. Merge the Branch
You can merge through a GitHub Pull Request, or locally:
```bash
git checkout main
git pull origin main
git merge feature/update-readme
git push origin main
```

## Important Git Commands

| Command | Purpose |
|---|---|
| `git init` | Creates a new Git repository |
| `git status` | Shows changed/untracked files |
| `git add .` | Stages changes |
| `git commit -m "message"` | Saves a version of the project |
| `git push` | Uploads local commits to remote repository |
| `git fetch` | Downloads remote changes without merging them |
| `git pull` | Downloads and merges remote changes |
| `git branch` | Lists or manages branches |
| `git checkout` | Switches branches |
| `git merge` | Combines changes from another branch |
| `git log` | Shows commit history |

## Fetch vs Pull
`git fetch` downloads changes from the remote repository but does not automatically merge them into the current branch.

`git pull` downloads remote changes and then integrates them into the current branch.

Therefore:
```text
git fetch = download only
git pull  = download + integrate
```
