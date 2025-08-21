# Gym-Git-Exercise-Solutions
This repo it contain all the Git related exercises in the  Gym training


// Bundle 1 exercises 1.


PS E:\TheGymTraining\Git exercises> git branch -m main master
PS E:\TheGymTraining\Git exercises> git branch
* master

PS E:\TheGymTraining\Git exercises> ^C
PS E:\TheGymTraining\Git exercises> git checkout -b dev
Switched to a new branch 'dev'
PS E:\TheGymTraining\Git exercises> git branch test
PS E:\TheGymTraining\Git exercises> git branch
* dev
  master
  test
PS E:\TheGymTraining\Git exercises> git checkout dev
M       README.md
Already on 'dev'
PS E:\TheGymTraining\Git exercises> git checkout test
M       README.md
Switched to branch 'test'
PS E:\TheGymTraining\Git exercises> git checkout dev 
M       README.md
Switched to branch 'dev'


PS E:\TheGymTraining\Git exercises> git status
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS E:\TheGymTraining\Git exercises> git branch -D test
Deleted branch test (was f3ec461).
PS E:\TheGymTraining\Git exercises> ^C
PS E:\TheGymTraining\Git exercises> 
PS E:\TheGymTraining\Git exercises> git add .
PS E:\TheGymTraining\Git exercises> git commit -m "bundle 1 exercises 1"
PS E:\TheGymTraining\Git exercises> git push origin dev


// Bundle 1 exercises 2.

PS E:\TheGymTraining\Git exercises> git stash
Saved working directory and index state WIP on dev: 8038649 readme uploaded to dev
PS E:\TheGymTraining\Git exercises> 

The stash entry is kept in case you need it again.
PS E:\TheGymTraining\Git exercises> git stash pop
README.md: needs merge
error: could not write index
The stash entry is kept in case you need it again.
S E:\TheGymTraining\Git exercises> git stash pop
CONFLICT (rename/delete): index.html renamed to home.html in Updated upstream, but deleted in Stashed changes.
CONFLICT (modify/delete): home.html deleted in Stashed changes and modified in Updated upstream.  Version Updated upstream of home.html left in tree.
On branch dev
Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add/rm <file>..." as appropriate to mark resolution)
        deleted by them: home.html


PS E:\TheGymTraining\Git exercises> git reset 
Unstaged changes after reset:
M       README.md
PS E:\TheGymTraining\Git exercises> 


// the bundel 2 exercises 1


  master
PS E:\TheGymTraining\Git exercises> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS E:\TheGymTraining\Git exercises> git add .
PS E:\TheGymTraining\Git exercises> git commit -m "service test"
[ft/bundle-2 d785cbf] service test
 1 file changed, 17 insertions(+)
 create mode 100644 services.html
PS E:\TheGymTraining\Git exercises> git push 
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.       

PS E:\TheGymTraining\Git exercises> git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 507 bytes | 507.00 KiB/s, done.     
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)    
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions
 * [new branch]      ft/bundle-2 -> ft/bundle-2
PS E:\TheGymTraining\Git exercises> 