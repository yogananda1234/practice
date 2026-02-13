                                         PART 2

When connecting local repo to remote repo we use the below command:
"git remote add origin "remote repo link" "

here, local repo is the project folder that is present on our local system where git is present, we give the command "git init" to initialise or to track the folder.

remote repo is the one hosted on the web, like GitHub, where we can upload all the files that is present on the local repo to the remote repo online.

origin is the nickname we give to the remote repo likewise it can be named anything.

> git remote:  this command shows us all the remote repos present on the current project

> git remote -v: this gives the url of the remote repo that is linked, and "v" 
                 stands for verbose.

eg: 
PS C:\Users\yoga\desktop\javascript\git-tutorial> git remote -v
origin  https://github.com/yogananda1234/practice.git (fetch)


> git remote remove origin: this removes the link between remote repo and the
                            local repo. 
                                                                          
after we link the local and remote repo, now the github starts to track the changes and branching.

And the important point to note is that github tracks the branching, and while we push the local repo to remote repo we push the branching that points to the latest commit.

> And after we make changes, everytime we have to push the changes to the git hub using the command "git push origin master", or else github would not recognise the changes and would be stuck in the previous commit or change.

> git push origin master --set-upstream: this sets up the shortcut for git push origin master, so you don't have to type this command again and agian to upload the changes, you can just type git push.

> git add . and git commit --amend -m "message here" commits the changes to the previous commit and does not create a new one.

> git push origin master -f:  here "master" is the branch and "-f" means fore push the changes, this is important to push the changes to github to previous commit. 

> git branch -a: shows us all the branches present on the github repo
> git switch "branch": this lets us switch to any branch we want to.

The github is also useful in downloading the git repositories in multiple systems, there are certain commands to do so

> git clone "--repo url--":  this command downloads the github repo to our local system.
> git fetch: This command lets us get the latest branch from the remote repo to github. Only updates the branches does not modify files.
> git pull: This command updates the changes, modify the files as well.