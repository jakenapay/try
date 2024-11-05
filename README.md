# Typical Git Workflow
1. **Clone the Repository**
    ```bash
    git clone <repo-url>
- This creates a local copy of the remote repository on your machine.

2. **Create a New Branch for Your Feature or Fix**
- Create a new branch for each new feature, bug fix, or task. This keeps changes isolated and organized.

    ```bash
    git checkout -b <feature-branch-name>
- Naming convention: Use descriptive names like feature/login-page or bugfix/footer-styling.

3. **Make Your Changes Locally**
- Edit, add, or remove files as needed in your feature branch.

4. **Stage and Commit Changes**
    ``` bash
    #Add files to the staging area:
    git add <file>        # Adds specific files
    git add .             # Adds all changes in the current directory

    # Commit your changes with a meaningful message:
    git commit -m "Add login page design"

5. **Regularly Pull Changes from the Remote Repository**
- Ensure your branch is up-to-date with the main branch to avoid conflicts.
    ```bash
    git pull origin main    # Replace `main` with the primary branch name if different
- If you’re on a feature branch, pull changes from the primary branch before continuing to work.

6. *Push Your Branch to the Remote Repository*
Push your branch to the remote repository, so others can review it.
    ``` bash 
    git push origin <feature-branch-name>

7. **Create a Pull Request (PR) / Merge Request (MR)**
- Go to your Git hosting platform (e.g., GitHub, GitLab, Bitbucket) and open a pull request (PR) to merge your feature branch into the primary branch (often main or master).
- Add a descriptive title and details about your changes in the PR description.

8. **Code Review and Address Feedback**
- Team members will review the PR, providing feedback and suggestions.
- Make necessary changes locally, commit them, and push them to the same feature branch.
- The PR will automatically update with these new commits.

9. **Merge the Pull Request**
- Once the PR is approved, it can be merged into the primary branch.
- Delete the feature branch (both locally and remotely) after merging to keep the repository clean:
    ```bash
    # Delete local branch
    git branch -d <feature-branch-name>
    # Delete remote branch
    git push origin --delete <feature-branch-name> 

10. **Pull the Latest Changes to Stay Updated**
- After merging, all collaborators should pull the latest changes from the primary branch to stay up-to-date:
    ```bash
    git checkout main
    git pull origin main
