## Git Configurations

```git
git config --global user.name "Your Name"
git config --global user.email "youremail@address.com"
git remote add origin 'https://github.com/yourgithub/reponame'
git config --list
```

Beware of this code:
```git
git config --global core.autocrlf true
```
## Basics


```git
git init
git add data-engineering-zoomcamp-2024
git commit -m "DE Zoomcamp 2024 Week 1 files, excluding postgresql volume data"
git push -u origin main
```

Create new branch
```git
git checkout -b main # or `git switch -c main`
```


### Other commands for troubleshooting:
```git
git ls-files --cached
git rm -r --cached .
git filter-branch --tree-filter 'sed -i -e "s/OLD_TEXT/REPLACEMENT_TEXT/g" ./path/to/file/text.md' HEAD
```


## Homework #1

Q1: --rm
Q2: 0.42.0



