# Git  exercise  project

## Bundle 1

### Exercise 1

``` bash
$ git status
On branch master
$ git branch -M main
$ git status
	On branch main
$ git add readme.md
$ git remote add origin git@github.com:haroldmud/git-practice.git
$ git push --set-upstream origin main
$ git checkout -b dev
	Switched to a new branch 'dev'
$ git checkout -b test
	Switched to a new branch 'test'
$ git push origin test
$ git branch -D test
	Deleted branch test (was 7ea8fc1).
$ git push origin --delete test
To https://github.com/haroldmud/Git-trial.git
 - [deleted]         test
 ```