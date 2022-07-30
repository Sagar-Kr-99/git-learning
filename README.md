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
13. git clone https://github.com/sagar-iitg/git-learning.git git-learning
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
20. git mv file.txt info.txt
21. git rm new1.txt
### if previously git is tracking file then command is to untrack file is:
22. git rm --cached file.txt
23. git rm --cached -f file.txt
### default branch is master

24. git log
25. git log -p
26. git log -p -3
27. git log --stat
28. git log --pretty=oneline
29. git log --pretty=short
30. git log --pretty=full
31. git log --since==2.days
32. git log --pretty=format:"%h --%an"
33. git log --pretty=format:"%h --%ae"
### unstaged file
34. git restore --staged <file>
35. git checkout -- <file>
36. git checkout -f
37. 





## clear git repository
1. rm -rf .git


