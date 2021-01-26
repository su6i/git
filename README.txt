git init
git status
git add FILENAME
git add -A or .                                           ----------> -A or just  ".": add all files	
git commit -S -m 'COMMENT'                                ----------> -m: Comment, -S: Signing
git log
git diff HEAD
git diff --staged
git reset FILENAME
git checkout -- FILENAME
git commit --amend                                       ----------> --amend: change the last commit message   
git branch
git branch BRANCHNAME
git checkout BRANCHNAME
git checkout -b BRANCHNAME                                ----------> -b: create a new branche and checkout into it
git merge BRANCHNAME                                      ----------> When we are in the master and want to merge files from other branches
git branch -d BRANCHNAME                                  ----------> remove a branch
git clone ADDRESS OF A GIT PAGE
git push -u origin master
git pull origin master
git config user.name "USERNAME"                           ----------> for just a repository
git config user.email "EMAIL ADDRESS"                     ----------> for just a repository
git config --global user.email                            ----------> for all repositories
git config --global user.name                             ----------> for all repositories
git config --global user.signingkey
git remote -v                                             ----------> -v: verbose
git remote add origin ADDRESS OF GIT's SITE
git show COMMIT HASH                                      ----------> for example: 4a7b7bad55a0a16409f6603592116cc5a20e95ab
git show VERSION                                          ----------> ex: git show v1.8, that shows signing message
git tag -v VERSION                                        ----------> Verifying the information of signature, -v: verify
git tag -a VERSION -m 'COMMENT'                           ----------> Create a version number for the last verified hash log, for ex: v2.0
git tag -a VERSION COMMIT HASH -m 'COMMENT'               ----------> ex: git tag -a v2.3 4a7b7bad55a0a16409f6603592116cc5a20e95ab -m 'myVersion 2.3'
git tag -s VERSION COMMIT HASH -m 'COMMENT'               ----------> -s: Sign the tag version
git push origin VERSION                                   ----------> Push tag version into remote (origin)
git push origin --tags
git checkout VERSION
------------------------------------------
gpg --list-keys
gpg --gen-key
gpg --list-secret-keys --keyid-format long                ----------> Create an electronic signature
git config --global user.signingkey SECRET KEY
------------------------------------------
git blame FILENAME -L8                                    ----------> Shows who wrote each line of the codes, -L: line's number like: -L8,10
------------------------------------------
git bisect start
git bisect bad                                            ----------> Find bugs
git bisect good
------------------------------------------ 
git help COMMAND                                          ----------> find help about a COMMAND, ex: git help remote
git ls-files -u 				                                  ----------> HashID of 3 stages
git pull remote master --allow-unrelated-histories        ----------> for resolving error "fatal: refusing to merge unrelated histories"
git merge source-branch && git branch -d source-branch    ----------> merge and delete a branch in one line
git push <remote_name> --delete <branch_name>             ----------> delete a remote branch
git config --global credential.helper store               ----------> Store user and password
------------------------------------------
git branch --merged master                                ----------> lists branches merged into master
git branch --merged                                       ----------> lists branches merged into HEAD (i.e. tip of current branch)
git branch --no-merged                                    ----------> lists branches that have not been merged
By default this applies to only the local branches. The -a flag will show both local and remote branches, and the -r flag shows only the remote branches.
------------------------------------------
git checkout --ours (theirs) FILENAME                    ----------> to resolve a conflict, when we want to use the file that is in our branch by --ours, and when we want to use the file that is in another branch with --theirs keyword
------------------------------------------
git fetch --all                                          ----------> Force tu pull from origin and overwrite all local files
git reset --hard origin/master
------------------------------------------
git rm --cached giant_file                               ----------> To remove a file from remote
git commit --amend -CHEAD
git push
------------------------------------------   
git submodule add https://github.com/example-username/example-repository   
 git diff --cached --submodule : If you don’t want to type `--submodule` every time you run git diff, you can set it as the default format by setting the `diff.submodule` config value to "log". `git config --global diff.submodule log`
 git commit -am 'Add example-repository module'
 
There is two to clone a repository with sub-modules:
 First way:
  git clone https://github.com/chaconinc/MainProject
  git submodule init
  git submodule update
 Second way:
 git clone --recurse-submodules https://github.com/example-username/MainProject
------------------------------------------
git checkout -b <new_branch> <commit_sha>                 ----------> To create a new branch from a commit 
