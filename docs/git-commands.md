# Git commands used in Experiment 1

Run these commands in the VS Code terminal from the relevant folder.

## Clone an existing GitHub repository
```bash
git clone https://github.com/kiranpatelkiran8197-rgb/Experiment-1-Git-Operations.git
cd Experiment-1-Git-Operations
code .
```

## Create, inspect, stage, and commit changes
```bash
echo "First tracked file" > first.txt
git status
git add first.txt
git status
git commit -m "Add first tracked file"
git status
```

## Push and pull
```bash
git push origin main
git pull origin main
```

## Initialize a separate repository
```bash
mkdir git-practice
cd git-practice
git init
git status
echo "Practice repository" > README.md
git add README.md
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-new-repository-url>
git push -u origin main
```

## Branch operations
```bash
git branch -a
git fetch origin
git switch -c feature-update
# Edit a file, then:
git status
git add .
git commit -m "Update project on feature branch"
git push -u origin feature-update
git diff main..feature-update
```

## Merge a branch locally
```bash
git switch main
git pull origin main
git merge feature-update
git push origin main
```

## Pull request workflow
Create a branch, commit and push its changes, then open a pull request on GitHub with:
- base: `main`
- compare: `pull-request-demo`

After reviewing, merge the pull request and update the local main branch:
```bash
git switch main
git pull origin main
git status
```
