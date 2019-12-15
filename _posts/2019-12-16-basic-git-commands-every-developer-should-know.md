---
title: "Basic Git commands: Every developer should know"
author: arasu_rrk
show_comments: true
permalink: "/blog/basic-git-commands-every-developer-should-know"
categories: [ Git ]
image: images/blog-hero/git.jpeg
tags: [git, featured]
---

[Git](https://en.wikipedia.org/wiki/Git) is a free and open-source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. 

Here are some basic GIT commands you need to know.

## Clone the Repository
----

###### Syntax
`git clone {url}` - Here `{url}` represents the Git Repository URL

###### Example
``` batchfile
git clone https://git.com/example/example-repository
```

By default, this command will clone the default branch of the repository (In most cases, the default branch is master).  If you want to clone a specific branch, follow the below syntax.

###### Syntax
``` batchfile
git clone {url} -b {branch_name}
```

###### Example
``` batchfile
git clone https://git.com/example/example-repository -b development
```

## Change Local Working Branch
----
To change the local working branch, use the `checkout` command.

###### Syntax
``` batchfile
git checkout origin/{branch_name}
```

###### Example
``` batchfile
git checkout origin/master
```

## Fetch changes from Remote
----
To fetch all changes from remote, use `fetch` command.

###### Syntax
``` batchfile
git fetch --origin
```

**NOTE:** This command will not merge the changes in the local branch. 

## Pull Updates from Remote
----

To update the local branch, use the following command.

###### Syntax
``` shell
git pull
```

## Merge changes from another branch
----

To merge the changes from another remote branch, use the following command. 

###### Syntax
``` batchfile
git pull --no-rebase "origin" {branch_name}
```

###### Example
``` shell
git pull --no-rebase "origin" development
```
This command pulls all the changes from the development branch and merges locally.

## Check the status of local changes
----
List the files you've changed and you need to add or commit:

###### Syntax
``` shell
git add {file_path}
```

## Stage your files
----
To stage your files, use the `add` command.

###### Syntax
``` shell
git add {file_path}
```

###### Example

1. To add the particular file.
   `git add test/file.md`

2. To add an entire folder
   `git add {folder_name}` - This will stage all the files in the corresponding folder. 

3. To add files by its extension.
   `git add *.{extension}` - `git add *.css` -> This will stage all files with .css extension. 

4. To add all files.
    `git add .` - This will stage all files.


## Commit changes
----

To commit the changes to remote, use the `commit` command. 

###### Syntax
``` batchfile
git commit -m "{message}"
```

###### Example
``` batchfile
git commit -m "Test commit"
```

> **NOTE**
> * Commit message is necessary for all commits. 
> * Changes will not be pushed to remote unless you push the changes to remote.

## Push changes to remote
----
To push the changes to remote, use the below command.

###### Syntax
``` shell
git push
```

## Revert all local changes
----
To revert all your local changes, use the below command.

###### Syntax
``` shell
git reset --hard
```

## To delete the unstaged files
----
To delete all the unstaged files, use the below command.

###### Example
``` shell
git clean -df
```

###### Options
* `-d` - To recurse the directories and delete.
* `-f` - Force delete. 


#### References
* <https://git-scm.com/docs>
* <https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html>
