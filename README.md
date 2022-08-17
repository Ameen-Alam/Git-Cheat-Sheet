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

  
#### To see from the Git history  
  
git merge --no-ff myfeature
  
  
#### Git  checkout from develop to new branch release-1.2
git checkout -b release-1.2 develop

  
#### The fix is by use autocrlf
git config --global core.autocrlf true

#### Renormalizing Line Endings
https://www.edwardthomson.com/blog/advent_day_21_renormalizing_line_endings.html
  
$ echo "* text=auto" >.gitattributes
$ git add --renormalize .
$ git commit -m "Introduce end-of-line normalization"


#### Git Troubleshooting
git bisect start
git bisect bad -< current commit
git bisect good hash
git bisect bad 
git bisect good
git bisect reset
git show hash
git revert hash

