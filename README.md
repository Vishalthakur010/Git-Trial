1. `git init` --> Powers your folder to be managed by git, and initiates a new empty repository.
it also creates a .git folder that has all the relevent logic to manage versions of your project.


2. `Working Area` --> There can be a bunch of files that are not currently handeled by git.
It means changes done in those files are not managed by git yet. A file which is in a working area 
considered to be not in the staging area. when we do 'git status' and we see a bunch of untracked 
files then these are actually called to be in the working area.


3. `Staging Area` --> What all files are going to be part of the next version that we will create.
This Staging area is the place where git knows what changes will be done from the last version
to the next version.


4. `repository Area` --> This area actually contains the details of all your previous registered
versions. And the files in this area, git already manages them and knows their version history.


5. `git add <file>` --> Moves file from working area to staging area.


6. `git rm --cached <file>` --> Moves file back from staging area to working area.


7. `commit` --> Commit is a particular version of the project. It captures a snapshot of the
project's staged changes and creates a version of it.


8. `git commit` --> Registers staged changes to a commit.


9. `git log` --> Lists down all the commits of the repository. If you want to exit out of git log
prompt, press 'q'.


10. `git restore <file>` --> It removes all file changes from the staging area to be commited.
This can be useful if we did some dirty piece of code and now no more want it. Instead of deleting 
every change line by line, we can restore it or you can say restore the last clean version of the file.
                        or
Removes changes from the working area.


11. `git restore --staged <file>` --> It moves file changes from staging area to the working area.
This only works when changes are in staging area.


12. Difference between git rm and git restore
Ans --> If you want to move the whole file to the untracked stage then we do git rm, or
if we want the changes to be moved in working area from the staging area then we do git restore.


13. `git diff commit1 commit2` --> gives the difference of all file changes between two commits.

14. `git commit -m "your commit message"`  --> Directly add commit message without opening any text editor. 

15. `git remote` --> list down all the remote connection names.

16. Remote connection --> It helps you link two git repositories for uploading and downloading changes
from each other.

17. `git remote add <name of remote> <link of remote>` --> This command help us to add a new link to the 
remote repo and give a name to it.

18. `git remote rm <name of remote>` --> Delete a remote connection.

19. `git remote rename <oldName> <newName>` --> Renames the remote connection.

note : The name of the remote connection is always used to establish communication between the repos.

20. `git add <file> <file> <file>` --> Adds multiple file changes together in the staging area.

21. `git add .` --> add all file changes from working area to staging area.

22. `git pull <remoteName> <branchName>` --> downloads latest changes from the branch of the mentioned 
remote to your local repo.

### recommended practice to do

    - make changes
    - git add <file>
    - git commit
    - git pull
    - git push