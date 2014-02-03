#Git Workshop

###Goals:
- Create new Github username
- Learn how to create repository on Github
- Initialize repository on computer
- Set remote repository to Github repo URL
- Add contents of new repository to commit
- Push up to master branch of Github repository

###First Steps:
Open terminal and follow instructions:

    cd ~
    mkdir git-todo
    cd git-todo

    touch README.md
    git init
    git add README.md
    git commit -m "initial commit"
    
###What Happened?
- `git init` creates a new repository in our `git-todo` directory. `cd git-todo` changes the directory into the `git-todo` directory. Think of it as going down one level.
- `touch README.md` generates a markdown file that is called README. 
- `git init` initializes, or generates, a new `.git` file. Think of a `.git` file as the memory store at the root of a directory. The logic that stores your repository data as well as the synchronization between your remote repositories is encapsulated in this `.git` file.
- Before you can commit new files, you have to "stage" them by adding them to a staging directory. You do this by `git add README.md`. You can also add all new/updated files in current directory by doing `git add .`, and if you also need to remove files that were deleted, you do `git add -A`
- Once all the previous steps are finished, you commit the staging file via `git commit -m "initial commit".
- Finally, push up to your remote via `git push origin master`.

