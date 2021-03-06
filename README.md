# dev-cheat-sheet
This information is intended for beginner or part-time developers who don't know the basic commands of the multiple tools and programming languages that they use by heart and sometimes need a little help. Goolge will of course also do the trick. :-)

## Table of Contents
- [Git](#git)
- [NPM](#npm)

## Git
### Basics
```bash
# Customize Git.
git config --global user.name "Charlie"
git config --global user.email "charlie.h@email.xx"

# Before Git can track your changes, you need to initialize the project folder.
cd folder-name
git init

# Do this always before invoking any of the below commands!
git status
```

### Project changes
```bash
# The first step is to stage changes.
# Stage a single file.
git add index.html

# Stage all files. (difference ???)
git add -A
git add .

# The second step is to commit the staged changes to your repo.
git commit -m 'Initial commit'

# This might come in handy if you have changed or deleted files by mistake or just want to revert your changes.
git checkout -- .
```

### Remote Repositories
```bash
# Check the remote repo url of your local project.
git remote -v

# Connect your local project to an empty GitHub repo.
git remote add origin https://github.com/efg/uuu-uu.git

# Clone an existing repo from GitHub.
git clone https://github.com/abc/aaa-aa.git

# Change the remote repo url of your local project.
git remote set-url origin https://github.com/efg/xxx-xx.git

# Push local repo to GitHub.
git push origin master

# Pull repo from GitHub
git pull origin master
```

## NPM
### Basics
```bash
# Initialize the folder as an npm project.
cd folder-name
npm init -y

# Install a single package.
npm install lodash

# A little shorter.
npm i lodash

# Install multiple packages.
npm i lodash express

# Install a specific version of a package.
npm i lodash@4.17.21

# Install packages used only for development.
npm i webpack webpack-cli --save-dev
```