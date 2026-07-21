# Upload This Release to GitHub

This folder is already arranged as a GitHub repository. Do not upload the ZIP
file as the only repository file. Extract it first, then upload the contents of
the extracted folder.

## Method 1: GitHub website

1. Create a new empty repository on GitHub.
2. Do not initialize it with another README, `.gitignore`, or license.
3. Extract `DXLR20-Control-Center-Complete-Release.zip`.
4. Open the extracted `DXLR20-Control-Center-Complete-Release` folder.
5. On the new GitHub repository page, choose **uploading an existing file**.
6. Drag the contents of the extracted folder into the browser.
7. Commit the files.

For a large number of files, the Git command-line method is more reliable.

## Method 2: Git command line on Windows

Open PowerShell in the extracted folder:

```powershell
cd "$HOME\Downloads\DXLR20-Control-Center-Complete-Release"

git init
git add .
git commit -m "Initial DX-LR20 Control Center release"
git branch -M main
git remote add origin https://github.com/YOUR-NAME/YOUR-REPOSITORY.git
git push -u origin main
```

Replace `YOUR-NAME` and `YOUR-REPOSITORY` with the real GitHub account and
repository name.

## Method 3: GitHub Desktop

1. Extract the ZIP.
2. Open GitHub Desktop.
3. Choose **Add an Existing Repository from your Hard Drive**.
4. Select the extracted folder.
5. Create the repository when prompted.
6. Publish it to GitHub.

## After upload

Confirm these links work on GitHub:

- `README.md`
- `START_HERE.md`
- `docs/index.md`
- `software/pi/install_complete_project.sh`
- `software/pc-gui/dxlr20_control_center.py`
- `software/heltec/Heltec_V3_Pi3B_Control_Remote_v3_3_Battery.ino`

The repository URL can then be shared as the full project link.
