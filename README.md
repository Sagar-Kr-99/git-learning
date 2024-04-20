# GIT-learning
Conflict Resoultion marker (<<< HEAD) 
## How to use .gitignore

###  ignore file error.log
1. error.log
### ignore multiple .log file
2. *.log
### ignore any directory/folder
3. dir/
### ignore only outter directory/folder
4. /dir/
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
37. git remote  
38. git remote add origin git@github.com:sagar-iitg/git-learning.git
39. git remote -v
### git alias
40. git config --global alias.st status 
41. git config --global alias.last 'log -p -1'
42. git config --global alias.unstage 'restore --staged --'
43. git branch
44. git config --global 
45. git stash
46. git stash pop
47. git checkout -b f2
### delete loccal branches
48. git branch -d f1
### delete remote branch
49. git push origin --delete f1
50. git push origin bugfix:mybugfix
51. 


### Branch Management
1. git branch
* master
  develop
  system

2. git branch -v
### already merged branches
3. git branch --merged
### not already merged branches  
4. git branch --no-merged
5. git branch -d develop
6. git branch -D develop
7.  
8. 




## clear git repository
1. rm -rf .git

## Remove directory from Git but NOT local
1. git rm -r --cached myFolder



## Forked Repo
1. 


