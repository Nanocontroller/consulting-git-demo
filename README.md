# consulting-git-demo

A practice repository for learning the Git workflow in VS Code: fork, clone, branch, commit, push, and pull request.

This repository contains no client code and no secrets. Please do not add any.

## Before you start

You need:

- Git installed (check with `git --version` in a terminal)
- VS Code installed, with your GitHub account signed in (Accounts icon, bottom-left)
- A GitHub account

## Step 1: Fork the repository

1. Open this repository on github.com.
2. Click **Fork** (top right), then **Create fork**.

You now have your own copy at `https://github.com/nanocontroller/consulting-git-demo`.

## Step 2: Clone your fork in VS Code

1. Press `Ctrl+Shift+P`, type `Git: Clone`, and press Enter.
2. Choose **Clone from GitHub**, then select `nanocontroller/consulting-git-demo`.
3. Pick a local folder, such as `C:\Source`.
4. When prompted, click **Open** to open the cloned folder.

Terminal equivalent:

```
git clone https://github.com/nanocontroller/consulting-git-demo.git
cd consulting-git-demo
```

## Step 3: Create your branch

Name your branch `yourname/add-intro`, using your first name in lowercase, for example `jane/add-intro`.

1. Click the branch name in the bottom-left status bar (it says `main`).
2. Choose **Create new branch**, type `yourname/add-intro`, and press Enter.

Terminal equivalent:

```
git switch -c yourname/add-intro
```

## Step 4: Edit your file

1. In the Explorer panel, open `team/` and then your file, such as `team/jane.md`. If your file doesn't exist yet, create it with the same name pattern.
2. Replace the placeholder line with one sentence about what you want to learn.
3. Save the file with `Ctrl+S`.

## Step 5: Commit your change

1. Open the **Source Control** panel (the branch icon in the left sidebar, or `Ctrl+Shift+G`).
2. Check the diff to confirm you changed only your file.
3. Click the **+** next to your file to stage it.
4. Type a message such as `Add learning goal for Jane` in the message box and press `Ctrl+Enter`.

Terminal equivalent:

```
git status
git add team/yourname.md
git commit -m "Add learning goal for yourname"
```

## Step 6: Publish your branch

1. Click **Publish Branch** in the Source Control panel.
2. If prompted to sign in, follow the browser sign-in, then return to VS Code.

Terminal equivalent:

```
git push -u origin yourname/add-intro
```

## Step 7: Open a pull request

1. Go to your fork on github.com. GitHub usually shows a banner for your new branch; click **Compare & pull request**.
2. Set the base repository to the original `consulting-git-demo` and the base branch to `main`.
3. Add a title such as `Add learning goal for Jane`, then click **Create pull request**.

## Stretch task: review a classmate's pull request

1. Open the original repository's **Pull requests** tab.
2. Open a classmate's pull request and click **Files changed**.
3. Hover over a line, click the **+** to add a comment, and click **Add single comment**.
4. Click **Review changes**, choose **Comment**, and submit.

## Troubleshooting

- **Sign-in prompt keeps appearing:** sign out of GitHub in VS Code (Accounts icon), then sign in again.
- **"Publish Branch" is missing:** make sure you are on your `yourname/add-intro` branch, not `main`.
- **"Nothing to commit":** confirm you saved the file (`Ctrl+S`) before staging.
- **Stuck:** post in the session chat or ask the person next to you.
