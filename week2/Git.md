Git Research

**1-:What is the origin??**

"origin" is the name of the remote repository where you want to publish you commits. 

-git clone https://github.com/gittower/git-crash-course.git
you'r saying to clone the repository from the origin

-git push origin branchname
you're saying to push to the origin repository.
 
**2-How can you find the current origin?**
    $ git remote show origin
    


![](https://i.imgur.com/ShvZR9k.png)

**How can you change the origin's url?**


The git "remote set-url" command takes two arguments:
1.An existing remote name(origin)
2.the new url

![](https://i.imgur.com/UDKB4wE.png)

**3- How to mege between 2 branches?**

$ git merge branch1 branch2.

**what happend if we do "git merge master current-branch"?**
=> it merge between the main and the current branch, and put it into the current branch (pull the main into the current branch).

**4-different uses of git-reset?**

$ git reset HEAD^ :remove the last commit.
& git reset HEAD^^ : remove the last 2 commits.


5-Talk about and give a demo of the following commands, when would you use each one?

git stash: remove all the updating in the document.

git log :After you have created several commits, or if you have cloned a repository with an existing commit history, you’ll probably want to look back to see what has happened. The most basic and powerful tool to do this is the git log command.

get fetch:The git fetch command only downloads the metadata associated with a project. 

---



