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


// Bundle 1 exercises 2


PS E:\TheGymTraining\Git exercises> git branch ft/service-redesign
PS E:\TheGymTraining\Git exercises> git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
PS E:\TheGymTraining\Git exercises> git add .
PS E:\TheGymTraining\Git exercises> git commit -m "services readisigning"
[ft/service-redesign bb2fbef] services readisigning
 1 file changed, 7 insertions(+)
PS E:\TheGymTraining\Git exercises> git push origin ft/service-redesign


PS E:\TheGymTraining\Git exercises> git diff main..ft/service-redesign
diff --git a/README.md b/README.md
index 1c2c9ee..2d6f833 100644
--- a/README.md
+++ b/README.md
@@ -106,4 +106,17 @@ remote:      https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions/pull/new
 remote:
 To https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions
  * [new branch]      ft/bundle-2 -> ft/bundle-2
-PS E:\TheGymTraining\Git exercises>
\ No newline at end of file
+PS E:\TheGymTraining\Git exercises> 
+
+
+// Bundle 1 exercises 2
+
+
+PS E:\TheGymTraining\Git exercises> git branch ft/service-redesign
+PS E:\TheGymTraining\Git exercises> git switch ft/service-redesign
+Switched to branch 'ft/service-redesign'
+PS E:\TheGymTraining\Git exercises> git add .
+PS E:\TheGymTraining\Git exercises> git commit -m "services readisigning"
+[ft/service-redesign bb2fbef] services readisigning
+ 1 file changed, 7 insertions(+)
+PS E:\TheGymTraining\Git exercises> git push origin ft/service-redesign
\ No newline at end of file
diff --git a/services.html b/services.html
index 81a948d..3e151de 100644
--- a/services.html
+++ b/services.html
@@ -8,19 +8,17 @@
   <body>
     <h2>Our Services</h2>
     <ul>
-      <p>We offer a variety of services to meet your fitness needs:</p>
+      <li>Personal Training</li>
       <li>Group Classes</li>
-      <div id="nk">how do you feel</div>
+      <li>Nutrition Coaching</li>
       <li>Online Coaching</li>
-      <li>Wellness Workshops</li>
-      <li>
-        <noframes><p>Mindfulness and Stress Management</p></noframes>
-      </li>
     </ul>
-    <p>
-      Our services are designed to cater to a wide range of fitness needs,
-      ensuring that everyone can find the right support for their journey.
-    </p>
-    <h3>this the different one i used for helping people</h3>
+    <h1> codebase</h1>
+    <div>
+      <p>
+        We leverage cutting-edge technology and a robust codebase to deliver
+        exceptional fitness solutions.
+      </p>
+    </div>
   </body>
 </html>
(END)

 E:\TheGymTraining\Git exercises> git diff main..ft/service-redesign
diff --git a/README.md b/README.md
index 1c2c9ee..2d6f833 100644
--- a/README.md
+++ b/README.md
@@ -106,4 +106,17 @@ remote:      https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions/pull/new
 remote:
 To https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions
  * [new branch]      ft/bundle-2 -> ft/bundle-2
-PS E:\TheGymTraining\Git exercises>
\ No newline at end of file
+PS E:\TheGymTraining\Git exercises> 
+
+
+// Bundle 1 exercises 2
+
+
+PS E:\TheGymTraining\Git exercises> git branch ft/service-redesign
+PS E:\TheGymTraining\Git exercises> git switch ft/service-redesign
+Switched to branch 'ft/service-redesign'
+PS E:\TheGymTraining\Git exercises> git add .
+PS E:\TheGymTraining\Git exercises> git commit -m "services readisigning"
+[ft/service-redesign bb2fbef] services readisigning
+ 1 file changed, 7 insertions(+)
+PS E:\TheGymTraining\Git exercises> git push origin ft/service-redesign
\ No newline at end of file
diff --git a/services.html b/services.html
index 81a948d..3e151de 100644
--- a/services.html
+++ b/services.html
@@ -8,19 +8,17 @@
   <body>
     <h2>Our Services</h2>
     <ul>
-      <p>We offer a variety of services to meet your fitness needs:</p>
+      <li>Personal Training</li>
       <li>Group Classes</li>
-      <div id="nk">how do you feel</div>
+      <li>Nutrition Coaching</li>
       <li>Online Coaching</li>
-      <li>Wellness Workshops</li>
-      <li>
-        <noframes><p>Mindfulness and Stress Management</p></noframes>
-      </li>
     </ul>
-    <p>
-      Our services are designed to cater to a wide range of fitness needs,
-      ensuring that everyone can find the right support for their journey.
-    </p>
-    <h3>this the different one i used for helping people</h3>   
+    <h1> codebase</h1>
+    <div>
+      <p>
+        We leverage cutting-edge technology and a robust codebase to deliver
+        exceptional fitness solutions.
+      </p>
+    </div>
   </body>
 </html>
(END)
-      </li>
     </ul>
-    <p>
-      Our services are designed to cater to a wide range of fitness needs,
-      ensuring that everyone can find the right support for their journey.
-    </p>
-    <h3>this the different one i used for helping people</h3>   
+    <h1>and codebase</h1>
+    <div>
+      <p>
+        We leverage cutting-edge technology and a robust codebase to deliver
+        exceptional fitness solutions.
+      </p>
PS E:\TheGymTraining\Git exercises> git diff ft/service-redesign..main
diff --git a/README.md b/README.md
index 2d6f833..1c2c9ee 100644
--- a/README.md
+++ b/README.md
@@ -106,17 +106,4 @@ remote:      https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions/pull/new
 remote:
 To https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions   
  * [new branch]      ft/bundle-2 -> ft/bundle-2
-PS E:\TheGymTraining\Git exercises>
-
-
-// Bundle 1 exercises 2
-
-
-PS E:\TheGymTraining\Git exercises> git branch ft/service-redesign
-PS E:\TheGymTraining\Git exercises> git switch ft/service-redesign
-Switched to branch 'ft/service-redesign'
-PS E:\TheGymTraining\Git exercises> git add .
-PS E:\TheGymTraining\Git exercises> git commit -m "services readisigning"
-[ft/service-redesign bb2fbef] services readisigning
- 1 file changed, 7 insertions(+)
-PS E:\TheGymTraining\Git exercises> git push origin ft/service-redesign
\ No newline at end of file
+PS E:\TheGymTraining\Git exercises> 
\ No newline at end of file
diff --git a/services.html b/services.html
index 3e151de..81a948d 100644
--- a/services.html
+++ b/services.html
@@ -8,17 +8,19 @@
   <body>
     <h2>Our Services</h2>
     <ul>
-      <li>Personal Training</li>
+      <p>We offer a variety of services to meet your fitness needs:</p>
       <li>Group Classes</li>
-      <li>Nutrition Coaching</li>
+      <div id="nk">how do you feel</div>
       <li>Online Coaching</li>
+      <li>Wellness Workshops</li>
+      <li>
+        <noframes><p>Mindfulness and Stress Management</p></noframes>
+      </li>
     </ul>
-    <h1> and codebase</h1>
-    <div>
-      <p>
-        We leverage cutting-edge technology and a robust codebase to deliver
-        exceptional fitness solutions.
-      </p>
-    </div>
+    <p>
+      Our services are designed to cater to a wide range of fitness needs,
+      ensuring that everyone can find the right support for their journey.
+    </p>
+    <h3>this the different one i used for helping people</h3>   
   </body>
 </html>
(END)



ft/team-page
// Bundle 3 exercises 1



PS E:\TheGymTraining\Git exercises> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS E:\TheGymTraining\Git exercises> git add . 
PS E:\TheGymTraining\Git exercises> git commit -m "team w html commit"
[ft/team-page f455c49] team w html commit
 2 files changed, 12 insertions(+)


PS E:\TheGymTraining\Git exercises> git log --oneline
2a99bff (HEAD -> ft/team-page, origin/ft/team-page) team w html committ
f455c49 team w html commit
ddd26b1 (origin/main, main, ft/contact-page) Update README.md
dadc857 Update README.md
bd39638 Delete wp
35700c6 (origin/ft/service-redesign, ft/service-redesign) Merge branch 
'main' into ft/service-redesign
e941d39 updated redme here
d15c9b0 change list to paragraph
79b8f31 services readisign with read me
bb2fbef services readisigning
801bf2a Merge pull request #1 from JEANPAUL-Rad/ft/bundle-2
f992d4d (origin/ft/bundle-2, ft/bundle-2) service include read me      
d785cbf service test
561ed68 (origin/dev, dev) uploading team
:


a303bdc Initial commit
PS E:\TheGymTraining\Git exercises> git revert 44f0e99
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not revert 44f0e99... using git log to see changes        
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".       
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".
hint: Disable this message with "git config advice.mergeConflict false"
PS E:\TheGymTraining\Git exercises> 

PS E:\TheGymTraining\Git exercises> git checkout -b ft/home-page-redesign
 ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

Switched to a new branch 'ft/home-page-redesign'
warning: cancelling a revert in progress
PS E:\TheGymTraining\Git exercises> git checkout -b ft/home-page-redesign
fatal: a branch named 'ft/home-page-redesign' already exists
PS E:\TheGymTraining\Git exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS E:\TheGymTraining\Git exercises> git add .
PS E:\TheGymTraining\Git exercises> git commit -m "adding 2 new paragraph"
[main 966d8e5] adding 2 new paragraph
 1 file changed, 3 insertions(+)
PS E:\TheGymTraining\Git exercises> git push main



// bundle 4 exercise 1


PS E:\TheGymTraining\Git exercises> git add .
PS E:\TheGymTraining\Git exercises> git commit -m "feat:pushing in changes in 2 different repository "
[main e647311] feat:pushing in changes in 2 different repository
 1 file changed, 4 insertions(+)

PS E:\TheGymTraining\Git exercises> git remote -v
git-copy        https://github.com/JEANPAUL-Rad/git-copy.git (fetch)
git-copy        https://github.com/JEANPAUL-Rad/git-copy.git (push)
origin  https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions (fetch)
origin  https://github.com/JEANPAUL-Rad/Gym-Git-Exercise-Solutions (push)
PS E:\TheGymTraining\Git exercises>

