# Git & GitHub Assignment
## Description
This repository demonstrates basic Git & GitHub workflow.
Git & GitHub Workflow (8-Step Guide)
Overview
This repository demonstrates a simple and practical Git & GitHub workflow using Git Bash. Follow all 8 steps to understand local version control, commits, and pushing to a GitHub remote repository.
STEP 1 — Create a folder, go inside it, and initialize Git
mkdir git-assignment && cd git-assignment
git init
STEP 2 — Configure Git (Run once on your computer)
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
STEP 3 — Create README.md (Commit #1)
echo "# Git & GitHub Assignment" > README.md
git add README.md
git commit -m "Commit 1: Add README file"

STEP 4 — Create a sample script (Commit #2)
echo 'print("This is sample data")' > sample_data.py
git add sample_data.py
git commit -m "Commit 2: Add sample_data.py script"
STEP 5 — Improve README.md (Commit #3)
echo "## Description" >> README.md
echo "This repository demonstrates basic Git & GitHub workflow." >> README.md
git add README.md
git commit -m "Commit 3: Add description to README"
STEP 6 — Add .gitignore file (Commit #4)
echo "__pycache__/" > .gitignore
git add .gitignore
git commit -m "Commit 4: Add .gitignore file"
Check your commit history:
git log --oneline
________________________________________
STEP 7 — Create a Public GitHub Repository
1.	Visit: https://github.com/new
2.	Enter a repository name: REPO_NAME
3.	Visibility: Public
4.	Do NOT check "Initialize with README"
You already created README locally.
________________________________________
STEP 8 — Connect local repo to GitHub and push
Replace:
•	GITHUB_USERNAME with your GitHub username
•	REPO_NAME with your new repository name
git remote add origin https://github.com/GITHUB_USERNAME/REPO_NAME.git
git branch -M main
git push -u origin main
Authentication instructions
If GitHub asks for login:
•	Username: Your GitHub username
•	Password: Your Personal Access Token (PAT)
(Not your GitHub password)
