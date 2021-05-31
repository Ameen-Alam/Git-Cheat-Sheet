# Git-Cheat-Sheet
Git-Cheat-Sheet

[Atlassian Git Cheat sheet](SWTM-2088_Atlassian-Git-Cheatsheet.pdf)

<br />

[Github Git Cheat Sheet](github-git-cheat-sheet.pdf)


#### Create empty branch on GitHub

$ git checkout --orphan empty-branch

$ git rm -rf .

$ git commit --allow-empty -m "root commit"

$ git push origin empty-branch


#### Recover deleted branch git

$ git reflog --no-abbrev
git checkout -b <your-branch> <sha>

#### Git Squash
  
git rebase -i HEAD~3
git merge --squash feature/login
