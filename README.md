✅ 1. Open Command Prompt or PowerShell

Press Win + R, type cmd, and hit Enter.
✅ 2. Navigate to the directory

cd "C:\Users\Kutan\Saved Games"

✅ 3. Initialize a Git repo (if not already)

git init

✅ 4. Add your GitHub remote

git remote add origin https://github.com/kutan16/saved-game-files.git

If you've already added it and it throws an error, run:

git remote set-url origin https://github.com/kutan16/saved-game-files.git

✅ 5. Add all the saved files/folders

git add .

✅ 6. Commit the files

git commit -m "Initial commit of saved game files"

✅ 7. Push to your GitHub repo

Since the GitHub repo is empty, you can force push to set the main branch:

git branch -M main
git push -u origin main

✅ 8. (Optional) Add a .gitignore file

If there are any files or folders you don’t want to upload (like temp files or crash logs), create a .gitignore before git add .

Example .gitignore:

*.tmp
*.log
