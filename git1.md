### &nbsp;                           PART-1



> **Git:**

&nbsp;     It is basically a version control system mostly used by programmers who collaboratively develop software, it is used to track the

&nbsp;     version of files, to keep a track on changes made by anyone, and allows programmers to contribute to any open source projects.

&nbsp;     And git is a software that can be installed on any local laptop.



> **GitHub:**

&nbsp;        It is a website, that is basically a platform that allows to create, store, manage, update, and share their code which can be  

&nbsp;        accessible to others. And the GitHub uses git software to use version control software.


Repository: It is nothing but a folder that is being tracked by git.


git init: to add git to a folder.  It is used to initialise git to a folder to keep track of changes.


git status: gets the status of all tracked and untracked files

ls: list

cd: change directory



git add: 1st step to add files, git add. adds all the files, and git add 
         "filename" adds a specific file to git.


git commit -m "--message--": commits the changes, along with the message to notify
                             what was changed.

git commit -m "--message--" --amend: this commits the changes to the previous commit
                                incase if we forgot to add the changes previously.


git tracks changes, not files.




after every commit we get a hash code that is called "commit hash"



git commit -m "message here" <filename>:   to modify specific file



staging area: Files that are added and are ready to be commited.

git status: to check the status of files

git log: 2s

git reset . : deletes the changes and gets back to working area from staging area.

git checkout -- . : deletes the changes and gets back from working area.4

git checkout "commit hash": the commit hash is like a key to a certain version, whenever you commit chnages, it generates a hash key, later we can use that
                            key to move to that version of the code.

git log --oneline:  to get all the list of changes that have been made in a compact way.



git log -p: this shows chnages made on each commit.



git log -p <filename>: this shows changes made to a particular file over the time.



git log --all: this shows all the commits made.

git log --all --graph: shows all the commits along with the branches.


"HEAD" shows which version or which stage we are in, it points to that.

"master" or "main" shows or points to the latest commit.

git checkout master: goes to the master branch.

git config --global user.name "Your Name"

git config --global user.email "your\_email@example.com"

The above both are used to set name and email 





git config --global alias.s "status":   Now this creates aliases or shortcuts for any command, in this case it is status, and this can be done to nay command



git status: this shows us the files that are being tracked, any commits thats has 
to be made.


 
dir -force:  to check if the "repo" or ".git" file is present or not

git rm --cached <filename>: to remove a file from repo

rmdir -Force -Recurse .git:  to remove the repo itself

shortcut for the above command is "rm -rf .git"



"insertions are nothing but number of lines added or inserted" 



git reset <file> or . : this resets the chan ges in staging area. Here "." means all



git checkout <file> or . : this completely erases the changes. Here "." means all
or we can make the changes by clicking on the integration that is provided next to the file when we hover over it





git log: to see the changes made by whom to which file on what time

q: to quit out of pager from log.

git branching: 

git --no-pager log:  to get the log details without the pager.





| You want to see...                | Command                           |

| --------------------------------- | --------------------------------- |

| All commits made, version history | `git log`                         |

| Compact commit list               | `git log --oneline`               |

| Changes in each commit            | `git log -p`                      |

| Changes in a specific file        | `git log -p <filename>`           |

| Unstaged changes                  | `git diff`                        |

| Staged changes                    | `git diff --cached`               |

| Everything (branches, graph view) | `git log --oneline --all --graph` |



git log --all --graph: this shows branching



git checkout <commit hash>:  This command is used to switch betwen version for previous changes, with this we can undo the changes that has been made recentky.



git commit -m "Updated index" <file1> <file2>:  This is used to commit any specific file and not whole folder.





git checkout master: gets back to recent commit.





git checkout <hash>           	Switches to that commit (detached HEAD).

git checkout <hash> .          	Replaces current files with versions from that commit but stays on the current branch.





git checkout<hash>: allows branching



git checkout <hash>.: does not allow branching, the head and master remain at the same place, that means they both do not change. Until the next change all the versions remain same, like this







PS C:\\Users\\yoga\\desktop\\HTML\&CSS-2\\project-youtube> git log --all --graph

\* commit 5b4c6216b01dfd8b4e46b03f849376c1991b0ea7 (HEAD -> master)

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:05:12 2025 +0530

|

|     Version 5

|

\* commit ae43287c8c2eb0942d1e3ec5c147fc6f78a27a4c

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:04:59 2025 +0530

|

|     Version 4

|

\* commit 8cb8ac143b56240f5fe88500fba7885aa83c45e8

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:04:00 2025 +0530

|

|     Version 3

|

\* commit 0b4c760e0525fbf5e976ae1bc91757cd25a5ca02

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:03:38 2025 +0530

|

|     Version 2

|

\* commit b6a71a4f8cd87a3462e170b2ed69837895929f75

&nbsp; Author: yogananda1234 <yoganandakv8@gmail.com>

&nbsp; Date:   Sun Oct 19 16:02:47 2025 +0530



&nbsp;     Version 1









Once the change is made it transforms, like this



PS C:\\Users\\yoga\\desktop\\HTML\&CSS-2\\project-youtube> git log --all --graph

\* commit 49f7122ea6731e254ca2d856be636e57d79aa0a6 (HEAD -> master)

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:07:38 2025 +0530

|

|     Version 1 updated

|

\* commit 5b4c6216b01dfd8b4e46b03f849376c1991b0ea7

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:05:12 2025 +0530

|

|     Version 5

|

\* commit ae43287c8c2eb0942d1e3ec5c147fc6f78a27a4c

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:04:59 2025 +0530

|

|     Version 4

|

\* commit 8cb8ac143b56240f5fe88500fba7885aa83c45e8

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:04:00 2025 +0530

|

|     Version 3

|

\* commit 0b4c760e0525fbf5e976ae1bc91757cd25a5ca02

| Author: yogananda1234 <yoganandakv8@gmail.com>

| Date:   Sun Oct 19 16:03:38 2025 +0530

|

|     Version 2






the below is an example of changing the contents of a particular version without branching.

PS C:\Users\yoga\desktop\javascript\git-tutorial> git add .
PS C:\Users\yoga\desktop\javascript\git-tutorial> git commit -m "version 1 restored"
[master 38b2edf] version 1 restored
 2 files changed, 2 insertions(+), 8 deletions(-)
PS C:\Users\yoga\desktop\javascript\git-tutorial> git log --all --graph
* commit 38b2edfe7d0f5b0be13eb862c49e4effb345c99b (HEAD -> master)
| Author: yogananda1234 <yoganadawk1020@gmail.com>
| Date:   Mon Feb 9 11:47:41 2026 +0530
|
|     version 1 restored
|
* commit 7ce7b8dec813886add0f528217d906ffa6366fe4
| Author: yogananda1234 <yoganadawk1020@gmail.com>
| Date:   Sun Feb 8 19:38:30 2026 +0530
|
|     version 4
|
* commit 72ed19fbcec91eea0b276f159b225a0a80e2b100
| Author: yogananda1234 <yoganadawk1020@gmail.com>
| Date:   Sun Feb 8 19:38:10 2026 +0530
|
|     version 3
|
* commit 4a83873e1d96e3fd59b0943178688989448bc503
| Author: yogananda1234 <yoganadawk1020@gmail.com>
| Date:   Sun Feb 8 19:37:40 2026 +0530
|
|     version 2
|
* commit 284aa73d29306c50b00e9832a98f8eb3a4f6e636
  Author: yogananda1234 <yoganadawk1020@gmail.com>
  Date:   Sun Feb 8 19:36:43 2026 +0530

      version 1
:














git checkout <commit> → You travel back in time and are standing inside that old photo. This allows branching



git checkout <commit> . → You copy that old photo and bring it into your current time, keeping your current position in the album. This doesn't allow branching















&nbsp;                                                      "MAIN COMMANDS part-1"







> create a version:

&nbsp;                  git init, git add, git commit -m "message", git status



> View pevious versions:

&nbsp;                  git log, git log --all --graph, git checkout <commit\_hash>, git checkout<branch\_name>











\[19-10-2025]: 





git reflog | grep "Version 2" :    It will show you when it was created and whether you later detached or reset HEAD around that time.



git cherry-pick 0b4c760e0525fbf5e976ae1bc91757cd25a5ca02:  That will re apply the Version 2 changes as a new commit on top of your current branch.



> git logs only show commits that are reachable from the current branch's HEAD



Git ignore: This file is creted just like git, it tells git not to track or ignore certain files that are mentioned in this file.











usage: git \[-v | --version] \[-h | --help] \[-C <path>] \[-c <name>=<value>]

&nbsp;          \[--exec-path\[=<path>]] \[--html-path] \[--man-path] \[--info-path]

&nbsp;          \[-p | --paginate | -P | --no-pager] \[--no-replace-objects] \[--no-lazy-fetch]

&nbsp;          \[--no-optional-locks] \[--no-advice] \[--bare] \[--git-dir=<path>]

&nbsp;          \[--work-tree=<path>] \[--namespace=<name>] \[--config-env=<name>=<envvar>]

&nbsp;          <command> \[<args>]






rm -rf .git or rmdir -force -recurse .git:  this removes the git repository from
                                            the folder.

dir -force: used to check if git repository exists or not.

A repository is nothing but a folder that keeps track of changes in the project






&nbsp;                               PART-2

&nbsp;                                                          



\[20-10-25]





Local repository(repo):  It is the one present on our computer and it known as "local"



Remote Repository:  It is the one present online, that can be accessed through web and it is known as "remote".



"~": tilda



git remote add origin <repo URL>:  This commands links both the remote repo and local repo,

&nbsp;                                 > remote refers to remote repo,

&nbsp;                                 > add means to add the repo,

&nbsp;                                 > origin, it is the name given to the remote repo, it can be named anything,

&nbsp;                                 <repo URL>, at this place we need to apply the url or link of the remote repo from github.



Branch or branches: A series of commits are called branch are branches



To check if the local repo is linked with remote repo, we have to give the command,



> git remote: this gives the name of the remote repo that we have set

> git remote -v: this shows the link or URL that we used to connecy local repo with remote repo, here "-v" stands for verbose, meaning get more info.



To remove or delete the remote repo, we should give the command,



> git remote remove <remote repo name>: this removes the remote repo.





To push our code or upload our code to the online repo or remote repo or to the Github, we use the command: 



> git push <remote repo name> "master" or "main":  here remote repo name is the name of the repo created by you on git hub, master or main is the latest commit.



&nbsp;"https://github.com/yogananda1234/Youtube-home-page.git" this is how a repo url looks like, if this doesn't work we can add our username in front of the github.com with an "@" like, " https://yogananda1234@github.com/yogananda1234/Youtube-home-page.git"



> After we push the commit to remote repo, the name of the repo like "origin" along with "master" that is the latest commit is displayed, like (origin, master)



> Create Access token  \[14:10]





> git push origin master --set-upstream: this is a shortcut for git push, so we don't have to type git push origin master everytime we commit, we can just give "git push".





"Overwriting a commit is not allowed"



> git fetch : This command brings all the changes, that is any new commits or any new updates from the remote repo to the local repo, but it does not apply it, it just shows it.



> git merge: This merges or includes the changes from remote repo to the local repo



> git pull: This is like "fetch + merge", this shows the changes and applies it to the local repo.

&nbsp; 

&nbsp; "git pull origin master", this is how it is written, here origin is the remote repo name, master is the latest commit made to the remote repo.

&nbsp; 

> The shortcut which we used for push can also be used here that is "git pull origin master --set-upstream", after writing this from next next we can just write "git pull" and it works

&nbsp; the shortcut for upstream is "-u"













&nbsp;                                                             



&nbsp;                                                        "MAIN COMMANDS part-2"







> Create an online backup(Github):

&nbsp;                           git remote add origin <repo URL>, git push origin <branch> in most cases it is main or master



> sync computer(local repo) to Github(remote repo):

&nbsp;                           git push origin <branch>, git push origin <branch> -f



> sync Github(remote repo) to computer(local repo):

&nbsp;                           git pull origin <branch>



function question(){
    console.log("Hey, did you receive the data")
}

function answer(){
    console.log("Yes received the data")
}

let promise = new Promise((resolve) => {
    setTimeout(() => {
        question(() => {
            resolve("End")
        })
    }, 2000-)
}).then((result) => {
    answer();
    console.log(result)
})

question()