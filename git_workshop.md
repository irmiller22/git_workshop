#Git Workshop

##Goals:
- Create new Github account
- Quick overview of Github

- Learn how to create own repository on Github +
- Initialize repository on computer +
- Set remote repository to Github repo URL +
- Add contents of new repository to commit
- Push up to master branch of Github repository

- Clone code from Github 
- Create new branch
- Change code around a bit
- Learn how to add files to staging area
- Commit on new branch
- Push code back to gihub

##First Steps:
Create New Github Profile:

		Go to https://github.com/
		Create a new account (username, email, password)
		When you confirm your account, it will redirect to the home page
		Click on the '+' sign next to your username in top right
		Select 'New Repository' 
		Give the repository the name 'git-todo'

Open terminal and follow instructions:

    cd ~/Desktop
    mkdir git-todo
    cd git-todo

    touch README.md
    git init
    git add README.md
    git commit -m "initial commit"
    git remote add origin <paste http:// link here from Github>
    git push origin master
    
###What Happened?
- `cd ~/Desktop` will change directory into our 'Users/<username>/desktop' directory
- `mkdir git-todo` will create a new folder called 'git-todo' on your Desktop
- `git init` creates a new repository in our `git-todo` directory. `cd git-todo` changes the directory into the `git-todo` directory. Think of it as going down one level.
- `touch README.md` generates a markdown file that is called README. 
- `git init` initializes, or generates, a new `.git` file. Think of a `.git` file as the memory store at the root of a directory. The logic that stores your repository data as well as the synchronization between your remote repositories is encapsulated in this `.git` file.
- Before you can commit new files, you have to "stage" them by adding them to a staging directory. You do this by `git add README.md`. You can also add all new/updated files in current directory by doing `git add .`, and if you also need to remove files that were deleted, you do `git add -A`
- Once all the previous steps are finished, you commit the staging file via `git commit -m "initial commit".
- Finally, push up to your remote via `git push origin master`.

##Next Steps:
- In this next step, we will clone a repository to our desktop, modify the file contents inside of the repository, commit those changes, and push back up to the `solutions` branch of the Github repository.
- Go to `https://github.com/irmiller22/git_workshop_test`.
- FORK this repository -- once the page reloads, the URL for your repository should be `https://github.com/<your-username>/git_workshop_test`.
- Clone your `git_workshop_test` repository via the HTTPS clone url option in the lower right hand corner of the Github repository screen.
- Switch over to your Terminal. 
- If you are not at your Desktop path, change directory via the following command: `cd ~/Desktop`.
- Then type in: `git clone <paste Github HTTPS URL here>`.
- Once completed, type `ls` to show all files/folders on your Desktop directory. You should see the `git_workshop_test` repository here.
- Change directory into the repo via `cd git_workshop_test`
- Open up the `assignment.md` file, and follow instructions there.

##OTHER RESOURCES:
###Getting Started
- [Getting Started 1](http://git-scm.com/book/en/Getting-Started-A-Short-History-of-Git)
- [Getting Started 2](http://git-scm.com/book/en/Getting-Started-About-Version-Control)

###Basics of Git
- [Git Basics 1](http://git-scm.com/book/en/Git-Basics-Recording-Changes-to-the-Repository)
- [Viewing The Commit History](http://git-scm.com/book/en/Git-Basics-Viewing-the-Commit-History)
- [Undoing Things](http://git-scm.com/book/en/Git-Basics-Undoing-Things)
- [Remotes](http://git-scm.com/book/en/Git-Basics-Working-with-Remotes)
- [Branches](http://git-scm.com/book/en/Git-Branching-What-a-Branch-Is)
- [Merging](http://git-scm.com/book/en/Git-Branching-Basic-Branching-and-Merging)
- [Branch Management](http://git-scm.com/book/en/Git-Branching-Branch-Management)
- [Workflows](http://git-scm.com/book/en/Git-Branching-Branching-Workflows)
- [Rebasing](http://git-scm.com/book/en/Git-Branching-Rebasing)

###Additional Resources
- [Git Guide](http://rogerdudler.github.io/git-guide/)
- [Think like a git](http://think-like-a-git.net/)
- [Git Branching](http://pcottle.github.io/learnGitBranching/)
- [Visual Git](http://marklodato.github.io/visual-git-guide/index-en.html)
- [Git ready](http://gitready.com/)



