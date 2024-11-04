# GIT Practice
# Hi, my name is jake!

<!-- # Create new file -->
# echo "message" >> <filename>
# touch <filename>

<!-- initialize the folder -->
# git init

<!-- add the files -->
# git add .
# git add <filename>

<!-- commit the tracked files -->
# git commit -m "message"

<!-- force rename and overwrite the existing main branch if existing -->
# git branch -M main

<!-- to add the remote repository to your local -->
# git remote add origin <remote URL>

<!-- your committed files will now push to main branch -->
# -u means upstream, use for first time push in remote branch
# git push -u origin main

<!-- to merge two branches -->
8. go to main branch
- git merge <merging branchname>