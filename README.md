# Creating a new repository from local machine using vs code editor and pushing it to github

Create a new repo from my local machine, it does not exist on github right now.
 we will create it, commit and push all the repo to the github account
 first write the command line:

 ```

 > git init
 ```

 write

 ```

 > git status
 ```

 you see will all the untracked files which is readme.md for now
 you have to stage all the untracked files by the command

 ```
> git add .
```

then write your first commit

```
> git commit -m "first commit from local repo"
```

lets push the committed files

```
> git push origin master
```

this will show an error because their is no such remote repo in the same name to push the files to, so we have to create an empty file in github and call it ' demo-repo2', then push the files to it using the following command

```
> git remote add origin https://github.com/Norhanms/demo-repo2.git
```

To show the repo changes write:

```
> git remote -v
```

Now you can push the files to the remote github repo

```
> git push -u origin master
```

this will create a branch called 'master' and push all the files to it.

From now you can write only

```

> git push
```

without the need to write origin master because when add the flag -u which means upstream which means push always to the same repo

## Branching

To show all branches in the repo, type in the following command:

```

> git branch
```

To create a new branch, type in the following command:

```

> git checkout -b feature-readme-instructions
```
 You are switched to work on this branch and if you showed all the existing branches, you will find that this branch is highlighted.
 Type in ``` git branch ``` again to see.

 To switch back to the master branch, type in:

```

> git checkout master
```

</br>

## Local development

1. create index.html file

## Unstaging changes

Type the command ``` git status ``` to see all the modified and new files that need to be statged.
You will find index.html is untracked because it is new and the readme file is modified.

lets learn how to unstage the changes but first we need to stage them.

```

> git add .

```

To unstage write :

```

>  git restore --staged .

```

Now lets enter to branch 'feature-readme-instructions'

```

> git checkout feature-readme-instructions

```

Write ``` git status ``` to check for the modified and new files that need to be staged

Stage and commit all the changes

```

> git add .
> git commit -m "updated the readme file with all the expliantion  and add index.html"

```

