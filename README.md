# GitHub
![octocat.png](https://raw.githubusercontent.com/LITTL3BEAR/foo/master/octocat.png)

## Create Command
$ echo "????" >> [file] _______________________________ : create file

$ git init ____________________________________________ : initial git

$ git add [file]

$ git status

// go to your github directory

$ config --global user.email "????"

$ config --global user.name "????"

$ git commit -m "????"

$ git remote add origin [url]

$ git remote -v

$ git push -u origin master ___________________________ : first upload

## Undo Command
$ git checkout [file] _________________________________ : discard edit

$ git reset HEAD [file] _______________________________ : discard add

$ git reset --soft "HEAD^" ____________________________ : discard top commit

$ git reset --soft [file] _____________________________ : discard commit

## branch Command
$ git branch -a _______________________________________ : list branch

$ git branch [???] _____________________________________ : switch to branch [???]

$ git checkout -b [???] ________________________________ : create brance & go to branch

$ git checkout master _________________________________ : switch to branch master

$ git merge --no-ff [???]

## Other Command
$ git clone [url] _____________________________________ : first download

$ git push ____________________________________________ : upload

$ git pull ____________________________________________ : download

$ git merge ___________________________________________ : compare

$ git fetch

$ git more [file] _____________________________________ : show

$ git add . ___________________________________________ : add all

$ git stash ___________________________________________ : hide update

$ git stash pop _______________________________________ : unhide update

$ git log _____________________________________________ : show all commit

$ git log --oneline

$ git rm [file] _______________________________________ : delete file

$ git config --global --unset user.name _______________ : logout

$ git config --global --unset user.email



