# git-details
Details Command GIT 
GiT Details .....

GitBash >...

 Git is a free, open source version control tool that developers install locally on their personal computers, 
 while GitHub is a pay-for-use online service built to run Git in the cloud. Git is a piece of software. 
 GitHub is an online SaaS service.
 
 1st : Go console ec2 instance of local linux server then use git command .

**SETUP**
 Configuring user information used across all local repositories
 git config --global user.name “[firstname lastname]”
 set a name that is identifiable for credit when review version history
 git config --global user.email “[valid-email]”
 set an email address that will be associated with each history marker
 git config --global color.ui auto
 set automatic command line coloring for Git for easy reviewing

  **SETUP & INIT**
 Configuring user information, initializing and cloning repositories
 git init
 initialize an existing directory as a Git repository
 git clone [url]
 retrieve an entire repository from a hosted location via URL

 **STAGE & SNAPSHOT**
 Working with snapshots and the Git staging area
 git status
 show modified files in working directory, staged for your next commit
 git add [file]
 add a file as it looks now to your next commit (stage)
 git reset [file]
 unstage a file while retaining the changes in working directory
 git diff
 diff of what is changed but not staged
 git diff --staged
 diff of what is staged but not yet committed
 git commit -m “[descriptive message]”
 commit your staged content as a new commit snapshot

 **BRANCH & MERGE**
 Isolating work in branches, changing context, and integrating changes
 git branch
 list your branches. a * will appear next to the currently active branch
 git branch [branch-name]
 create a new branch at the current commit
 git checkout
 switch to another branch and check it out into your working directory
 git merge [branch]
 merge the specified branch’s history into the current one
 git log
 show all commits in the current branch’s history

**  SHARE & UPDATE**
 Retrieving updates from another repository and updating local repos
 git remote add [alias] [url]
 add a git URL as an alias
 git fetch [alias]
 fetch down all the branches from that Git remote
 git merge [alias]/[branch]
 merge a remote branch into your current branch to bring it up to date
 git push [alias] [branch]
 Transmit local branch commits to the remote repository branch
 git pull
 fetch and merge any commits from the tracking remote branch

 ** REWRITE HISTORY**
 Rewriting branches, updating commits and clearing history
 git rebase [branch]
 apply any commits of current branch ahead of specified one
 git reset --hard [commit]
 clear staging area, rewrite working tree from specified commit

** TEMPORARY COMMITS**
 Temporarily store modified, tracked files  in order to change branches
 git stash
 Save modified and staged changes
 git stash list
 list stack-order of stashed file changes
 git stash pop
 write working from top of stash stack
 git stash drop
 discard  the changes from top of stash stac

 ** TRACKING PATH CHANGES**
 Versioning file removes and path changes
 git rm [file]
 delete the file from project and stage the removal for commit
 git mv [existing-path] [new-path]
 change an existing file path and stage the move
 git log --stat -M
 show all commit logs with indication of any paths that moved
