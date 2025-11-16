


# VCS Task – Git Commands Practice (Merge, Rebase, Stash)

This repository contains practice work for learning Git basics such as creating files, branching, merging, rebasing, stashing, and pushing to GitHub.

---

## 📁 Step 1: Create Files Using Shell

```bash
echo "Hii this kaviya. i want to file in script" > script1.sh
echo "India is my country. i love tech. i want to be a architecture." > script2.sh
ls

🧱 Step 2: Initialize Git Repo
git init
git add .
git commit -m "i added two script files in sh"

🌐 Step 3: Connect to GitHub
git remote add origin https://github.com/kaviyapalanivel-src/vcs-task.git
git branch -m main
git push --set-upstream origin main

🌿 Step 4: Create New Branch and Commit
git checkout -b new-branch
echo "this is next branch file" > script3.sh
git add script3.sh
git commit -m "This next my next branch"
git push -u origin new-branch

🔀 Step 5: Merge Branch Into Main
git checkout main
git merge new-branch
git push

🔁 Step 6: Rebase Practice
git checkout -b rebase-branch
echo "this is my another new branch for rebase" > sript4.sh   # (typo kept same)
git add sript4.sh
git commit -m "This is rebase branch i added 4th script file"

git checkout main
git checkout rebase-branch
git rebase main


Push after rebase:

git push --set-upstream origin rebase-branch

📦 Step 7: Stash Practice
echo "i added this line of script1 file" >> script1.sh
git stash
git stash list
git stash apply
git stash drop

🧹 Step 8: Final Commit and Push
git add .
git commit -m "i create branch perform, rebase and merge"
git push

📁 Step 9: Create Screenshot Folder
mkdir screenshot
git add .
git push origin main

📜 Final Git Log Example

You verified the log using:
git log

git log
