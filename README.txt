1. 'git init' --> Powers your folder to be managed by git, and initiates a new empty repository.
it also creates a .git folder that has all the relevent logic to manage versions of your project.


2. 'Working Area' --> There can be a bunch of files that are not currently handeled by git.
It means changes done in those files are not managed by git yet. A file which is in a working area 
considered to be not in the staging area. when we do 'git status' and we see a bunch of untracked 
files then these are actually called to be in the working area.


3. 'Staging Area' --> What all files are going to be part of the next version that we will create.
This Staging area is the place where git knows what changes will be done from the last version
to the next version.


4. 'repository Area' --> This area actually contains the details of all your previous registered
versions. And the files in this area, git already manages them and knows their version history.

5. 'git add <file>' --> Moves file from working area to staging area.

6. 'git rm --cached <file>' --> Moves file back from staging area to working area.