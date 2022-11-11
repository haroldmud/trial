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

 ### Exercise 2

 ```bash
 $ git status
        home.html
$ git stash list
$ git add home.html
$ git status
        new file: home.html
$ git stash
	Saved working directory and index state WIP on dev: 7ea8fc1 init project
$ git stash list
	stash@{0}: WIP on dev: 7ea8fc1 init project

$ git add about.html
$ git status
        new file: about.html
$ git stash
$ git stash list
stash@{0}: WIP on dev: 7ea8fc1 init project
stash@{1}: WIP on dev: 7ea8fc1 init project

$ git add team.html
$ git status
        new file: team.html
$ git stash
$ git stash list
stash@{0}: WIP on dev: 7ea8fc1 init project
stash@{1}: WIP on dev: 7ea8fc1 init project
stash@{2}: WIP on dev: 7ea8fc1 init project

$ git stash pop stash@{1}
        new file:   about.html
	Dropped stash@{1} (04355e17a24a059308ef9b64abb73fd8400314de)
$ git stash pop stash@{2}
        new file:   home.html
	Dropped stash@{1} (04355e17a24a059308ef9b64abb73fd8400314de)
$ git stash
$ git status
	new file:   team.html
$ git reset --hard
	HEAD is now at 0359eee Stash pop the about and the home page
    ```
```
	
## Bundle 2

### Exercise 1
```bash 
$ git checkout -b ft/bundle-2
	Switched to a new branch 'ft/bundle-2'
$ git add services.html
$ git commit -m "Create the service page"
$ git push origin ft/bundle-2 
```
