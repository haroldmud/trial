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
## Bundle 2

### Exercise 2
```bash 
$ git checkout main
	Switched to the branch 'main'
$ git checkout -b ft/service-redesign
	Switched to a new branch 'ft/service-redesign'
$ git add services.html
$ git commit -m "feat: add services list"
$ git push
$ git checkout main
	Switched to the branch 'main'
$ git add services.html
$ git commit -m "feat: add old services list"
$ git merge main
	Auto-merging services.html
```

## Bundle 3

### Exercise 1
```bash 
$ git status
	On branch main
$ git checkout -b ft/team-page
$ git add .
$ git commit -m "feat:create the team page"
$ git push origin ft/team-page
$ git checkout main
$ git checkout -b ft/contact-page
$ git checkout ft/team-page
$ git log
$ git cherry-pick beb88b8068906372ae6675ad296238927dd82814
	[ft/contact-page dd6d5da] feat: Create the team page
 	Date: Fri Nov 11 17:35:53 2022 +0200
 	1 file changed, 12 insertions(+)
 	create mode 100644 team.html
$ git add --all
$ git push origin ft/contact-page
$ git checkout -b ft/faq-page
$ git add --all
$ git commit -m "feat: Add faq page"
$ git push origin ft/faq-page
$ git log
$ git revert dd6d5daa5a4a0df69bafd4a01a7ff114e8942985
	This reverts commit dd6d5daa5a4a0df69bafd4a01a7ff114e8942985.
$ git push
``` 
## Bundle 3

### Exercise 2
```bash 
$ git checkout -b ft/home-page-redesign
	Switched to a new branch 'ft/home-page-redesign'
$ git checkout main
	Switched to branch 'main'
$ git commit -m "Update the home.html file"
$ git checkout ft/home-page-redesign
$ git rebase main
$ git add .
$ git commit -m "Add the menu to home.html"
$ git push --set-upstream origin ft/home-page-redesign
``` 

## Bundle 4

### Exercise 1
```bash 
$ git checkout main
$ git remote add git-copy git@github.com:haroldmud/git-exercise-clone.git
$ git remote
	git-copy
	origin
$ git push origin
$ git push git-copy
``` 

### Exercise 2
```bash 
$ git checkout -b ft/footer
	Switched to a new branch 'ft/footer'
$ git add .
$ git commit -m "Add footer page content"
$ git push --set-upstream origin ft/footer
$ git commit -m "Add a navigation bar"
$ git push
$ git checkout main
$ git checkout -b ft/squashing
	Switched to a new branch 'ft/squashing'
$ git merge --squash ft/footer
$ git commit -m "future changes squashing"
$ git push --set-upstream origin ft/squashing
```

## Bundle 4

### Exercise 1
```bash 
$ git commit -m "feat: Rename home to index"
$ deployed link: https://haroldmud.github.io/Git-trial/
``` 
### Exercise 2
```bash 

``` 