# GIT ASSIGNMENT PART - 3

# PART - 1 : Git Commit Basic
   # I  have created an folder on my local system (git_hotwax)
   # git init                            :  Intialize a git repository.
   # echo "Hello developer! > file2.txt  :  Through this command creating a file2.txt.
   # git add file2.txt                   :  Through this command adding changes made in file2.txt.
   # git commit -m "Add file2.txt"       :  Commiting the file2.txt.
   # git log                             :  Veiwing commit history.

# PART - 2 : Reverting a Commit
   # echo "Another change " >> file2t.xt : Making new changes in file2.txt.
   # git add file.txt                    : Adding new changes.
   # git commit -m "Add another change"  : Commiting the changes made.
   # git revert HEAD                     : This command is used to revert or go back to the last commit we made.
   # git log                             : This command is used to check  the history of the commits.

# PART - 3 : Merge conflicts
  # git branch branch1                  : Creating branch1
  # git branch branch2                  : Creating branch2
  # git checkout branch1                : Switching to branch1
  # echo "Change from branch1" >> file2.txt   : Changes made in file2.txt which is at branch1.
  # git commit -am "Update file in branch2"   : Adding and commiting changes made in file2.txt at branch1.
  # git checkout branch2                      : Switching to branch2.
  # echo "Change from braqnch2" >> file.txt   : changes made in file2.txt which is at branch2.
  # git commit -am "Update file in branch2"   : Adding and commiting changes made in file2.txt at branch2.
  # git checkout branch1                      : Swtiching to branch1.
  # git merge branch2                         : Attempt to merge branch2 into branch1.
  # git add file.txt                          : Resoving the conflict occurs in the file2.txt (manually) then adding it.
  # git commit 

# PART - 4 : Cherry-Picking Commits
   # On branch1,creating a new commit-
   # echo "Cherry-pick this commit" >> file.txt
   # git commit -am "Add cherry-pick commit".

   # Switching to branch2 and cherry-pick the commit-
   # git checkout branch2
   # git cherry-pick 35ee570 - After resolving the conflicts the system shows as many hints pick any of the you want like if want you to continue the add the change and run "git cherry-pick --cintinue", or if you want to skip it use "git cherry-pick --skip" , or want to abort and get back to the state before "git cherry-pick" the run "git cherry-pick --abort" .
   # git add file2.txt
   # git cherry-pick --skip

# PART -5 : Fetching Branches
  # Adding a remote repository-
  # git remote add origin https://github.com/Sandhyajaiswal203/hotwax_git.git .

  # Fecting branches-
   # git fetch
   # git branch -r

# PART - 6 : Sycing forked branch
   # This is done in my remote repository where i forked my friends repository and feching it and making changes in it and by pull reguest sending it to marge the changes made my me.
   # It can also be done through commands -
   # git remote add upstream <upstream-repo-URL>     : Here upstream means the original repository which you want to fork.
   # git remote -v                                   : Verfiy the Remote Repositories or to confirm that upstream is added.
   # git fetch upstream                              : Fetchupdates from upstream repository into your local repository.The fetched chnges will be stored in alocal branch upstream/main or upstream/master.
   # git merge upstream/master                       : Merge the fetched updates from the upstream branch into your working branch.

# PART- 7 : Merging via Command Line
  # Creating and merging branches-
  # git branch feature-branch
  # git checkout feature-branch
  # echo "Feture work " >> file2.txt
  # git commit -am "Add feature work"
  
  # git checkout main
  # git merge feaute-branch

# PART - 8 : Git Stash
   # Mdofiying a file but don't commit-
   # echo "Temporyary changes" >> file2.txt
   # git stash : Used to stash file

   # Veiw stashed changes-
   # git stash list : This will list stashed files

   # Apply the stash -
   # git stash apply

# PART - 9 : Pushing to Remote
   # Push changes to Github from local- 
   # git remote add origin <link> : Setting or adding Remote Repository.
   # git remote -v : To verify remote
   # git branch : To check branch status
   # git push origin master : Pushing local repository on Github.

# PART - 10 : 
   # Push changes to Github -
   # git push -u origin master.
  
# PART - 11 : Rebasing Branches
   # Create
