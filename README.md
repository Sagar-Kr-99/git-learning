# GIT-learning

## How to use .gitignore

###  ignore file error.log
1. error.log
### ignore multiple .log file
2. *.log
### ignore any directory/folder
3. dir/
### ignore only outter directory/folder
3. /dir/
### git ignore blank folder by default


# GIT Commands

1. git config --global user.email "enter your email id"
2. git config --list
3. git config --global core editor emacs
4. git config --global core editor vim
5. git config user.name
6. git config user.email
7. git status
8. git init

#### --a means all
9. git add --a
10. git add .

11. git commit -m "msg"
12. git log
13. git clone https://github.com/sagar-iitg/git-learning.git
#### comparing working directory to staging area
14. git diff 
#### comparing previous commit to current staging area(green color) --> modified
15. git diff --staged
### skipping staging area
16. git commit -am "msg"
### How do I get the Git commit count?
17. git rev-list --count HEAD
18. git rev-list --count master 
### To get the commit count across all branches:
19. git rev-list --all --count 
20. 



## .git folder
1. du -c
2. 
## clear git repository
1. rm -rf .git


