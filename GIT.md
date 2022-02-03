# Git Commands

```
$ git config –-global user.name "Your Name"     // Sets user name in git system
```
```
$ git config -–global user.email "your_email@mail.com"     // Sets user e-mail in git system
```
```
$ git init –-bare [NOMEDOPROJETO].git     // Initializes a new versioning git project
```
```
$ git clone "PATH_URL"     // Clones default project path
```
```
$ git remote add origin "PATH_URL"     // Sets project folder like original main project path

Note: To update source repository:
$ git remote set-url origin "https://github.com/.../project-name.git"
```
```
$ git pull origin "BRANCH"     // Update the repository branch with the last branch version of source repository
```
```
$ git add "file_name.js"     // Add file with changes uncommited to a staged file area

Note: To add all files together:
$ git add . (change the file name for a dot)
```
```
$ git commit -m "commit message"     // Commit stagged files
```
```
$ git push -u origin [BRANCH]     // Send the last modifications that are in HEAD index repository from selected branch to source branch project
```
```
$ git checkout [BRANCH]     // Changes branch from working to selected
```
```
$ gitk     // Open git default interface
```
