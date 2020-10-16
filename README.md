# Github_CheatSheet

# Setup:

git config --global user.email "mail"

git config --global user.name "name"

# Commands:

git init                       ==> creates a new Git repository

git status                     ==> List which files are staged, unstaged, and untracked.

git add file                   ==> The git add command is used to add file contents for the next commit.

git add --all                  ==> The git add command is used to add files content for the next commit.

git commit -m "commit message" ==> moves files from staging to the repository and records the time/date, author and a commit message that can be used to add additional context.

.gitignore                     ==> To ignore these files you create a .gitignore file in the root of the repository.

'''
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
'''

git diff ==> enables you to compare changes in the working directory.

git dif file       ==> enable you to compare changes in a file.

git diff commit    ==> enable you to compare changes in a commit.

git difftool      ==> Launch extenal tool to compare changes.

git diff --staged  ==>  compare the changes in the staging area against the previous commit.

git mv file1 file2 ==> mv contents of one file to another.

git rm file         ==> To remove a file from working directory.

git log             ==> view the history of the repository and the commit log.

git show <commithash>   ==> view the changes made in the commit
