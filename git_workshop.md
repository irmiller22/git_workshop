#Git Workshop

###Goals:
- Create new Github username
- Learn how to create repository on Github
- Initialize repository on computer
- Set remote repository to Github repo URL
- Add contents of new repository to commit
- Push up to master branch of Github repository

##First Steps:

###Creating New Github Profile:
- Go to `https://github.com/`
- Create a new account (username, password, email)
- Look in the top right corner where your username is
- Click on the `+` to the right of the username
- Click on `New Repository`
- You will be taken to the repository creation page
- Type in `git-todo` as the name of the repository
- Leave it as a Public repository, and leave the box unchecked for `Initialize this repository with a README`
- Then click on the `Create Repository` button

###Adding the Remote to Your Local Repository
- From the repository screen, copy the https://.... link and switch to your terminal
- Follow the instructions in the next section

###Creating the New Git-Todo Directory
Open terminal and follow instructions:

    cd ~
    mkdir git-todo
    cd git-todo

    touch README.md
    git init
    git remote add origin https://.....
    git add README.md
    git commit -m "initial commit"
    git push origin master
    
###What Happened?
- `git init` creates a new repository in our `git-todo` directory. `cd git-todo` changes the directory into the `git-todo` directory. Think of it as going down one level.
- `touch README.md` generates a markdown file that is called README. 
- `git init` initializes, or generates, a new `.git` file. Think of a `.git` file as the memory store at the root of a directory. The logic that stores your repository data as well as the synchronization between your remote repositories is encapsulated in this `.git` file.
- `git remote add origin ...` adds the HTTPS link to your Github repository that you just created; this is required so that you may store your data in your local repo on your remote repo, and thus have a version control management filesystem
- Before you can commit new files, you have to "stage" them by adding them to a staging directory. You do this by `git add README.md`. You can also add all new/updated files in current directory by doing `git add .`, and if you also need to remove files that were deleted, you do `git add -A`
- Once all the previous steps are finished, you commit the staging file via `git commit -m "initial commit".
- Finally, push up to your remote via `git push origin master`.

