# Git global setup
```sh
git config --global user.name ""
git config --global user.email ""
```
# Create a new repository
```sh
git clone url_git
cd test
git switch -c main
touch README.md
git add README.md
git commit -m "add README"
git push -u origin main
```
# Push an existing folder
```sh
cd existing_folder
git init --initial-branch=main
git remote add origin url_git
git add .
git commit -m "Initial commit"
git push -u origin main
```
# Push an existing Git repository
```sh
cd existing_repo
git remote rename origin old-origin
git remote add origin url_git
git push -u origin --all
git push -u origin --tags
```