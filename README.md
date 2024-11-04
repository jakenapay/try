# GIT Practice
### Hi, my name is jake!

<!-- # Create new file -->
1. echo "message" >> <filename>
- touch <filename>

<!-- initialize the folder -->
2. git init

<!-- add the files -->
3. git add .
- git add <filename>

<!-- commit the tracked files -->
4. git commit -m "message"

<!-- force rename and overwrite the existing main branch if existing -->
5. git branch -M main

<!-- to add the remote repository to your local -->
6. git remote add origin <remote URL>

<!-- your committed files will now push to main branch -->
7. -u means upstream, use for first time push in remote branch
- git push -u origin main