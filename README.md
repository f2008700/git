# git gyaan


Important links
http://markjberger.com/git-tips-for-beginners/

Git diff between two commits on a folder
http://stackoverflow.com/questions/12123633/differences-for-a-certain-folder-between-git-branches

Git with Meld
http://stackoverflow.com/questions/2006032/view-differences-of-branches-with-meld
sudo apt-get install meld
git config --global merge.tool meld
https://stackoverflow.com/questions/19830464/git-cherry-pick-and-conflicts


See changes between two commits: 
http://stackoverflow.com/questions/1191282/how-to-see-the-changes-between-two-commits-without-commits-in-between

Git Ignore all except
http://stackoverflow.com/questions/987142/make-gitignore-ignore-everything-except-a-few-files


Multiple users with git
https://stackoverflow.com/questions/4220416/can-i-specify-multiple-users-for-myself-in-gitconfig

Git open in folder format
https://stackoverflow.com/questions/7897517/why-does-git-difftool-not-open-the-tool-directly


Switch Branch 
git checkout <branch name>

Git pull with unsaved changes
git stash 
git pull
git stash pop

https://stackoverflow.com/questions/23517464/error-cannot-pull-with-rebase-you-have-unstaged-changes/23517639


Git remove local changes
git checkout /path/to/file
git checkout -- .

Create a new branch
git checkout -b <Branch name>
git pull origin trunk
git push --set-upstream origin trunk_BID-6549

Squash commit
git commit --amend
BID-6549: Type message here


Git see last commit
gd `git log | head -n 1 | awk '{print $2}'`^!

Git Delete a branch
git branch -d <Name of  branch>
git branch -D <Name of banch> 
https://stackoverflow.com/questions/2003505/how-do-i-delete-a-git-branch-both-locally-and-remotely

Git diff
Between two branches
git difftool --dir-diff trunk..trunk_BID-6549
Uncommitted changes
gd
For the last commit
	gd `git log | head -n 1 | awk '{print $2}'`^!
Change in a specific commit
git diff <Hash of the commit>^!


Git log local branch changes
https://stackoverflow.com/questions/4649356/how-do-i-run-git-log-to-see-changes-only-for-a-specific-branch
git log trunk..

Git import change from another branch (Check what is the difference between this and cherry pick)
https://stackoverflow.com/questions/2474353/how-to-copy-commits-from-one-branch-to-another
	
Apply a specific commit:
https://stackoverflow.com/questions/9339429/what-does-cherry-picking-a-commit-with-git-mean
Steps:
Go the branch on which you want to apply the patch to
git cherry-pick  <commit-hash>



Git merge voes
git mergetool
https://stackoverflow.com/questions/26376832/why-does-git-say-pull-is-not-possible-because-you-have-unmerged-files

git branch off from current branch
git pull origin trunk
git merge it to the actual branch 
git push

https://stackoverflow.com/questions/19830464/git-cherry-pick-and-conflicts
git cherry-pick ....
git mergetool
git cherry-pick --continue




Remove commits upto something specific
https://stackoverflow.com/questions/1338728/delete-commits-from-a-branch-in-git

Git branch - details (tag something along with a branch)
https://stackoverflow.com/questions/15058844/print-branch-description

Go back before merge step
https://stackoverflow.com/questions/6006737/git-merge-errors

Get another branch completely
git checkout origin/rel-1.1.6

Git correct merge history 
When there are multiple commits and you want to put only one commit in the history
git rebase -i HEAD~2

https://stackoverflow.com/questions/5189560/squash-my-last-x-commits-together-using-git


Git show the base of a branch
git log --oneline --graph --all --decorate
