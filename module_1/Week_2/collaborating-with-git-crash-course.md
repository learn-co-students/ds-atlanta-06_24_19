## My partner(s) and I are about to start a new project. What do we do?
One of you should create the repository. The owner of the repo should click the "Settings" tab (small gear icon) at the top of the page on github.com, then click "Collaborators and Teams", then _add the other team member as a collaborator on the repo_. This will give the collaborator _write_ access, that means they can push directly to the repository.

The partner should _clone_ this repository, _not fork it_. When you fork something it is like maintaining an entirely separate copy. Your team should have one repository (a single source of truth) that all members are collaborating on using git.

Once the project is done, if the team member who did not create the repo would like to have a version of it on their own github page (ie github.com/my-github-username/name-of-project) that would be a good time to fork it. All team members should have a robust commit history on the project so it should be clear that everyone contributed. (See below) 

## So, I wrote some code, I tested it, and I'm ready to push my changes. Now what?

## Step 1: Commit

First thing you'll have to do is commit your changes. This is like saving them and adding them to the history of all changes that were made.

##### What do I do if:
- I'm on my own feature branch, separate from master
  * `git add .` then `git commit -m "Did the thing."`
- Woops, I'm still on `master`, I forgot to make a new branch
  * No worries, _your changes follow you around to whatever branch you switch to until you make a commit_
  * Create a new branch with `git checkout -b my-feature-branch-name`. The `-b` stands for branch and you'll only need to do this _the first time you create a new branch_. After that you can switch between branches with `git checkout name-of-branch`. If you have the Learn bash profile setup you can use the `co` shortcut `git co name-of-branch`. Then commit like normal.
- I'm not sure what branch I am on
  * Again, no worries, if you are using the default Learn bash profile, the word you see above your bash prompt next to the blue timestamp that is red and wrapped in parentheses is the name of the current branch you are on.
  * Additionally, you can always run either `git status` or `git branch` and it will tell you the current branch you are on
- I'm not sure if I already committed
  * At any point in time you can run `git status` and see if you have changes that have not been committed. ("Changes not staged for commit" means you haven't run `git add` yet, the adding part is referred to as "staging", committing is just called committing)

## Step 2: Make sure your code includes all of the most up to date code

Before you push your code up, you want to be sure that your branch includes all of the changes that any other team members may have pushed during the time it took you to complete your feature.

- Switch back to the `master` branch using `git checkout master`
- Run `git pull` to get any and all changes that have been added to `master` since the last time you pulled. Now your local master is up to date with the remote master.
- Switch back to your feature branch with `git checkout name-of-my-branch`
- Locally _merge master into your feature branch_ with `git merge master` (while on that separate branch). This will make sure that when you push changes they will include _all of the current code_ *plus* _any changes you made_.  This will also give you the opportunity to locally fix any merge conflicts so that the whole team doesn't need to do that multiple times. In the files specified in your terminal, examine and resolve any merge conflicts in your text editor if prompted, i.e. if any merge conflicts exist.

## Step 3: Your local branch is ready to be pushed, so push it to the remote (ie on github.com) repo

After making sure everything still works after you have merged in master and fixed any conflicts, you can be assured that your code is ready to be pushed.  At this point your feature branch exists locally, It may or may not exist on github.com (this is what is known as the _remote_ repo).

##### What do I do if:
- The branch does not exist on the remote. This is the first time you are pushing this branch
  * `git push -u origin name-of-my-branch`. The `-u` stands for "upstream". Basically, you are associating your local branch with the remote branch of the same name. You'll only have to do this the first time.
- The branch already exists on github.com. I had to make another commit to add some changes. Even if you have already opened a PR, it's ok to make another commit.
  * In this case you can just run `git push`, or if you like verbosity, run `git push origin name-of-my-branch`. Because your local branch is "tracking" the upstream branch, `git push` is sufficient, it's a shorthand for `git push origin whatever-branch-im-on`

## Step 4: Open up a Pull Request (PR)

Now your code is on the internet. Usually, if you visit the repo online, GitHub will show a message saying you recently pushed a branch. You can click that if you see it. If not you can click the dropdown of all the branches and find your branch there.

After selecting your branch, You want to click to create a "New Pull Request" and keep clicking through the menus while adding any comments you would like to add.

The Pull Request is how you are sharing your changes with the team.  It wouldn't be very nice or polite if you showed up tomorrow to work on your project and all the code was different and you didn't know about any of the changes. You don't want to put your teammate in that position.

You can tag your teammate as a reviewer, in which case they will receive an email that there is a PR that is awaiting their review, or send them a slack with a link to the PR. Or do both!

You want to give everyone on the team a chance to view the changes, understand and digest them, add any comments they may have, either request some changes or approve and acknowledge that they have seen the changes.

If your teammate requests changes you can start the process over from Step 1. If your changes are approved, you can go ahead and advance to the following step.


## Step 5: Merge the PR

Your changes have been approved :tada: and your teammate has left an encouraging message! You are now ready to merge your branch into master. Do this through the interface on github.com. On the PR page, click to merge the branch into master.


At this point, for any subsequent changes you basically begin the process over. If your teammate has some changes they want to push. They should start with Step 1, then move to Step 2 where they will get _all of your changes_ and then add in theirs, and so on.
