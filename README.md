# Git Commands and Setup

## Initializing and Working with Branches

1. **Initialize a Branch:**
   ```sh
   git init

2. **Add Files:**
   - Add a specific file:
     ```sh
     git add file_name
     ```
   - Or add all files in the current directory:
     ```sh
     git add .
     ```
   - Or add all files, including those in subdirectories:
     ```sh
     git add *
     ```
3. **Commit Changes:**
   ```sh
   git commit -m "add a message"
4. **Check the Current Branch:**
   ```sh
   git branch
5. **Create a New Branch:**
   ```sh
   git branch "branch_name"
6. **Switch to Another Branch:**
   ```sh
   git checkout "branch_name"
7. **Check Where HEAD is Pointed:**
   ```sh
   git log --oneline
8. **Merge a Branch:**
   ```sh
   git merge branch_name
9. **Delete a Branch:**
   ```sh
   git branch -d branch_name
10. **Compare with Previous Stage in the Same Branch:**
    ```sh
    git diff --staged
    ```
11. **Save Work Without Commit (Stash):**
    ```sh
    git stash
    ```
12. **Retrieve Stashed Data:**
    ```sh
    git stash pop
    ```
13. **Rebase Command:**
    - Note: The rebase command should not be used in the master branch; it can be used in other branches.
14. **Set Up Your SSH Key:**

   ```sh
   # a) Open Git Bash
   git bash

   # b) Generate an SSH Key
   ssh-keygen -t ed25519 -C "your_email@example.com"

   # c) Copy the SSH Key
   clip < ~/.ssh/id_ed25519.pub
   # (This command copies the SSH key to your clipboard.)

   # d) Open GitHub Account Settings
   # - Go to your GitHub account settings.

   # e) Click on SSH and GPG keys

   # f) Click on New SSH key

