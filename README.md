echo "# git" >> README.md
git init // initial the repo locally
git add README.md // add a file to the staging history
git commit -m "first commit" // commit the file from staging
git branch -M main // first time change to main
git remote add origin https://github.com/spacewitch123/git.git // add origin to identify the matching repo from local to remote
git push -u origin main // push to main with setting the upstream only first time


// main commands

** commiting **
git add . // stage the directory
git add file_name // stage the file

git commit -m "message to identify the commit" // commit all the staged 

** checking the history before commiting or at any time
git status // shows the staged and untracked files
// staged means not commited yet but add to the staging phase
git log // log the commits by history

** moving around
two branches for exampe branch main and branch other
git remote -v // list the origin of the local repo (which repo it connects to in github)
git branch -r // list all the branches in remote repo in red including yours but in green
git branch // list all the branches in local repo in red including yours but in green
// checkout from main to other
git checkout other
// chekcout from main to non existing branch which mean create then checkout in one command
git checkout -b new_branch

** flow of creating a branch + commiting + pushing for first time based on main branch **
git checkout -b other
git add .
git commit -m "testing commit"

git push -u origin other // first time only set upstream
git push //

git diff // to know what you just changed but the files has to be non-staged first git add .
