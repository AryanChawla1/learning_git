# learning_git

How to go about starting git and github

## Why use Git?

Version control system to easily track changes made locally and remotely for files, directories, and projects. Especially when working in a team, overwritting changes is a mess, it's better to be able to work independently on a local version (repository), then push changes for everyone to see (remote respository).

Github is a service that hosts the respositories online to allow collaboration. Git and Github work together to allow you to access them and make changes without disrupting everyone else.

A respository are folders/directories with git intialized to allow the useful stuff to work!!

## Downloading and Installing Git

This is different based on operating systems...

The first thing to do is check if you have it already. Run the following command in your terminal:

```
git --version
```

If you have it will say the version, if not it will prompt you (for Mac??). If not use this link and it should work: https://git-scm.com/download/win

## Creating Github Repository

Go to your github account and click "Respositories". Then click "New". Make sure to add a README.md as it gives info about your project.

This is the remote respository. Notice the README.md file and above it there is a label saying main and 1 branch.

Git utilizes a tree structure to optimze teamwork. This is so members can branch off to work on individual aspects and once ready and tested, merge them back into the where they started. This is the purpose of the main branch, seemingly the origin and finality of all the work done.

## Adding Repository Locally using Git

Before we actually clone the repository, we will first configure our identity, this is important for Git to know who is making changes and if you are allowed to make changes.

Run the following command. Make sure you use the email assigned with GitHub.

```
git config --global user.name <name>
git config --global user.email <email>
```

Now on Github, click the green "Code" button and copy the link for HTTPS. Now in the terminal:

```
git clone <link>
```

This will create the git repository in your directory. Verify it's there and open the folder.

## Git Commands

We will go over the following commands:

- git status
- git add
- git commit
- git push
- git pull
- git checkout
- git rebase
- merging we will do through GitHub :D

One thing to understand when changing your work. Saved local changes are not included for git. For the changes to be considered they must be added. Once added they can be committed. Then once all your changes are done, you can commit your changes. Notice, however, this only done locally. It is not yet reflected on GitHub. For this to be reflected their, you need to push the commits. This will push the changes to the remote repository.

Now if I were to make changes, for other users to see the changes on their local repository, they need to pull the changes from GitHub to their local repository.

The checkout and rebase are for working with branches. Checkout allows you to create, access, and delete branches, while rebase is a bit more complicated, essentially updating the version of the code you made your changes on.

## Adding the HTML page

Let's create an HTML page and add it to the remote respository. I'm calling it index.html. I have also added text to the README.md file.

In the HTML file, type html:5 and it should auto-generate some code for you. I added a heading with hello world.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>
```

Let's reflect this remotely. First we will use this command:

```
git status
```
