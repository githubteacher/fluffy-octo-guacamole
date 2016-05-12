Welcome to Teacher!

We'll be using Gitter, a chat service that integrates with GitHub, for Q&A. Please click the button below to join the chat room for today's class.


[![chat room](https://badges.gitter.im/githubteacher/fluffy-octo-guacamole.svg)](https://gitter.im/githubteacher/fluffy-octo-guacamole?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

### Useful Links
- [GitHub Guides](https://guides.github.com)
- [StackOverflow Git Tagged Questions](http://stackoverflow.com/questions/tagged/git)
- [xkcd](https://xkcd.com/54/)

Notes from Day 1, section 1:

![alt tag](https://imgs.xkcd.com/comics/git.png)

### Getting Ready for Class
- Make sure you have [Git insalled](https://git-scm.com/) on your computer and a [GitHub account](https://github.com/).

### Getting Started
**Quick review of what we've covered so far:**
- Repository for Class: https://github.com/githubteacher/developers-may-2016
- Tour of Repository:
  - Code View:  Files belonging to the project
  - README.md: Description of the Repository
  - Issues: A place to have conversations and collaborate
  - Pull requests: A place to collaborate while introducing changes to your project
- Comment on [this issue](NEWLINKHERE) to become a collaborator on the project
- Practice making an issue [in the issues tab of the class repository](NEWLINKHERE).
  - For today's activity, be sure to include your username in the title, like "YourUserName Hometown"
  - In the body of the issue, we added the steps we'll take for the workflow.
  - Our goal later will be to add a document with information about your hometown, like good restaurants or things to do.
  - You can include [markdown](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf) syntax here.

**Getting access to the collaborator script:**
The collaborator script is open-source! You can access it [here](https://github.com/github/training-utils). Our [training kit](https://github.com/github/training-kit) is also open-source. We invite you to use these and welcome contributions to both these repos!

### GitHub Flow
**You can find that visual of the GitHub flow at this link:** https://guides.github.com/introduction/flow/

### Branching with Git
**Review of branches**
- When you create a branch, you are essentially creating an identical copy of the project at that point in time that is completely separate from the master branch.
- Create a branch on GitHub.com in the class repository
  - Click the 'branch' dropdown
  - Enter a branchname name 'firstname-lastname-hometown'


### Local Git Configs
**Review of configurations:**
- We determined our git version by running `git --version`... version 1.9+ is recommended
- If you need to, you can install it [here](https://git-scm.com/)
- If you don't already have GitHub Desktop, you can install it [here](https://desktop.github.com/)
- Clone the repository by running `git clone https://github.com/githubteacher/developers-may-2016.git` (Make sure you are in the directory where you want the repository to be when you run this command)
- Set up your Git configurations by running these commands:
  - `git config --global user.name "your name"`
  - `git config --global user.email <youremail@email.com>`
  - `git config --global core.editor <editor>` (For more help associating your text editor with Git, read [this GitHub Help article](https://help.github.com/articles/associating-text-editors-with-git/).
  - `git config --global push.default simple`
  - Windows ONLY: `git config --global core.autocrlf true`
  - Mac and Linux ONLY: `git config --global core.autocrlf input`
- Check your configurations by running `git config --list`

### Working Locally
**Review of working locally**
- Working on our new branch, we created a new file.
- List the files in your current directory by running `ls -la`
- We learned about 'working', 'staging', and 'history' and how commits fit into those areas using [this resource](https://services.github.com/kit/modules/CONT-CLI-04_Two_Stage_Commit.html).
- See your working/staged area  `git status`. This command is :heart:!

Notes from Day 1, section 2:

### Using Git Locally
- Change your file from 'working' to 'staging' by running `git add <file-name>`
- Change your file from 'staging' to 'history' by running `git commit`. (To avoid using the text editor, use `git commit -m "Enter commit message here"`)
- Text editor opens: Write a 'commit message' tells a story of the changes you just made in 50 characters or less.
- List the files in your current directory by running `ls -al`
- We learned about 'working', 'staging', and 'history' and how commits fit into those areas using this resource.
- Create a new file and repeat steps 1 - 3 for the two stage commit. This way, we'll have two commits to work with.
- Here are some shortcuts to know about in the future:
  - To automatically stage all files that have been changed, run `git add -A`. _Note: This will only work for files that are already being tracked, not brand new files._
  - Avoid the text editor in the commit by running `git commit -m "commit message"`

### Collaborating on Code
- Review of moving from Git to GitHub
- We talked about remote, and how we can see details about it by running `git remote`, `git remote -v`, and `git remote show origin`
- 'Push' our changes on the current branch to GitHub.com by running `git push -u origin <branch-name>`
- If you forget the `-u` tag, set a 'upstream branch' relationship between our local branch and the GitHub.com remote branch by running `git branch --set-upstream-to=origin/<remote-branch-name>`
- This means we only have to run git push and git pull in the future
- `git pull` is the combination of `git fetch` and `git merge`
- `git branch` and `git branch -a` will help you see what is going on with your local and remote branches
- On GitHub.com, open a pull request in our class repository by clicking the green "New pull request" button.
- Make sure your pull request says "Base: master" and "Compare: <your-new-branch>"
- Give it a good title and message about the changes you introduced. Bonus points for using markdown and emojis!
- You can add labels and assignees to pull requests like we did with Issues.
- Using @mention is important - you can mention people or teams to give them a notification to see your pull request to start collaboration.

### Notifications
- Notifications are an important part of GitHub. You can customize these several ways.
  - For GitHub in general, Settings/notificatons
  - For repositories, at the top of a repository page on GitHub.com by clicking "Watch"
  - For individual issues and pull requests by clicking "unsubscribe" on the right hand side of the webpage
- On the pull request page, we talked about the different tabs for 'conversation', 'commits', and 'files changed'.
  - 'Conversation' is where you and your colleagues can collaborate on your changes. This view includes comments as well as notes of when changes happen.
  - 'Commits' shows a history of what commits were added - this is why your commit messages matter - they tell a story.
  - 'Files changed' will let you see the actual code in several different formats. You also can make line level comments from this view.

Notes from Day 1, section 3:
### Collaborate on GitHub
- Once you've opened a pull request, go into someone else's. Please don't merge someone else's PR.
- Look at their code, and make a comment about something you see.

### Merging Pull Requests
- During class, please do not close or merge any pull requests other than your own.
- On your own pull request, if all is green and there are no conflicts, go ahead and merge your branch.
- After merging a branch, it's part of the master branch and good practice is to delete it.
- This is a major difference between Git and some older version control systems. In Git, branch, merge, and delete branches often.
- Back at the command line, we need to pull down the changes from GitHub.com in the remote repository.
  - `git checkout master`
  - `git pull`
  - `git branch --merged`
  - `git branch -d <branch-name>`
  - `git fetch --prune`
Configure your settings to do this by default by typing `git config --global fetch.prune true`

### View Local Changes
- Use `git log` to view the history of the repository
- `git log` will show commits from your own local repository, but also changes made by other collaborators
- Experiment with different option switches to view history:
  - git log
  - git log --oneline
  - git log --oneline --graph
  - git log --oneline --graph --decorate
  - git log --oneline --graph --decorate --all
  - git log --stat
  - git log --patch
- Use the up and down arrows or press enter to view additional log entries. Type q to quit viewing the log and return to the command prompt.

### Streamline Workflow With Aliases
- Set up an alias in configurations: `git config --global alias.<desired-alias> "the long version of the command that you want the alias to run, without git at the beginning, and with the desired flags"`

lets see what happens with the conflict
