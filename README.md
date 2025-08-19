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