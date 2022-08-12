# Demo 2

create a new repo from my local machine, it does not exist on github right now.
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

this will create a branch called 'master' and push all the files to it
