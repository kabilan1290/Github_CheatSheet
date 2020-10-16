# Github_CheatSheet

# 🔧 Setup:

git config --global user.email "mail"

git config --global user.name "name"

# ℹ️️ Commands:

git init                       ==> creates a new Git repository

git status                     ==> List which files are staged, unstaged, and untracked.

git add file                   ==> The git add command is used to add file contents for the next commit.

git add --all                  ==> The git add command is used to add files content for the next commit.

git commit -m "commit message" ==> moves files from staging to the repository and records the time/date, author and a commit message that can be used to add additional context.

.gitignore                     ==> To ignore these files you create a .gitignore file in the root of the repository.

```
Example:
echo ".tmp" > .gitignore
git add .gitignore
git commit -m ".gitignore"
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore

echo "test" > 1.tmp
git status
On branch master
nothing to commit, working tree clean

Sometimes there are particular files or directories you never want to commit, such as local development configuration.To ignore them we use .gitignore.In the above example 1.tmp is ignored.
```

git diff ==> enables you to compare changes in the working directory.

git dif file       ==> enable you to compare changes in a file.

git diff commit    ==> enable you to compare changes in a commit.

git difftool      ==> Launch extenal tool to compare changes.

git diff --staged  ==>  compare the changes in the staging area against the previous commit.

git mv file1 file2 ==> mv contents of one file to another.

git rm file         ==> To remove a file from working directory.

git log             ==> view the history of the repository and the commit log.

git show <commithash>   ==> view the changes made in the commit.
 
git pull                ==> allows you to sync changes from a remote repository into your local machine.

git push                ==> Push changes to the repository.

git fetch               ==> helps the user download commits, refs, and files from the remote repository to the local repository.

git merge               ==> to merge changes we fetched from git fetch.
```
git pull is a combination of git fetch+git merge
```
git mergetool   ==> External tool to review merge conflicts.

git checkout            ==> undo changes

git reset                ==> move files back from the staging area to the working directory(unstaged).

git reset --hard         ==> combination of git reset and checkout.

git revert               ==> Used to undo a commit so you can return a repository to the previous commit. 

git rebase               ==> the process of moving or combining a sequence of commits to a new base commit.

git rebase --interactive ==> We can interactively edit the history.

git pull --rebase        ==> to avoid conflicts when u made some changes in local repo.

git branch test          ==> creates a branch test.

git checkout test        ==> Switching to branch named test.
Switched to branch 'test'

git checkout -b test     ==> create and checkout to branch test.

git branch -a             ==> List branches

```
Example for merging a branch to master banch.
$ git checkout master
Switched to branch 'master'
$ git merge test
Updating 87a57f5..7a8812e
Fast-forward
 test.txt       | 1 +
 staging.txt    | 2 +-
 2 files changed, 2 insertions(+), 1 deletion(-)
 create mode 100644 new-file-6.txt
 ```
git branch -d test       ==> Delete branch named test.

git log --oneline        ==> Commit overview in short view.

git log -p               ==> git log with commit history.

git log -p -n 2          ==> git log with commit history(Number of commits to display -n 2)

git bisect               ==> Command allows to do binary search.

git blame file           ==> shows the revision and author who last modified each line of a file.

git cherry-pick          ==> Mege individual commits.

**Never presume to know a person based on the one dimensional window of the internet. A soul can’t be defined by critics, enemies or broken ties with family or friends ❤.**
