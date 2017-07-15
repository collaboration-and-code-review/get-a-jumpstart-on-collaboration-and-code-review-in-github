# Get a Jumpstart on Collaboration and Code Review in GitHub

<!--
https://2017.djangocon.us/speaking/speaker-resources/#slide-guidelines
https://docs.google.com/presentation/d/16LvCzF1mywdEvhXwUyJCdEuyiw05q-ITGiJEgFT6L-Y/edit#slide=id.g20735b3908_0_0
-->

This is a transcript of a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) will give at [DjangoCon](https://2017.djangocon.us), [PyLadies Remote](http://remote.pyladies.com), and other events.

<!--
* [Original slide deck]()
* [Video recording]()
-->

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

## Transcript

<table>


<tr><td width="30%">

![Slide 1]()

</td><td>

### Get a Jumpstart on Collaboration and Code Review in GitHub 

By Katherine "Kati" Michel

</td></tr>


<tr><td width="30%">

![Slide 2]()

</td><td>

### Welcome 

Thank you for being here. I'm thrilled to have the opportunity to talk to you about getting a jumpstart on collaboration and code review in GitHub

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### About Me 

* DjangoCon Website Chair (where I learned a lot of what I"m going to be teaching you)
* DjangoCon Europe Website Committee Member
* DEFNA (Django Events Foundation North America) Board Member
* Project Manager
* Web Designer and Developer

I hope you've had a chance to take a good look at the DjangoCon website. I'm so proud of what the team has accomplished. It's truly a beautiful website.

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### The Journey and Destination

Let’s pretend we’re going on a journey. The journey is to learn collaboration and code review. I've made this Journey Before. When you are making a journey, often you are engrossed in each step. When you complete the journey, looking back, perhaps you see the larger picture and have learned something. If I were to start my journey of learning collaboration and code review over again, knowing what I know now, I would do things differently from the beginning. 

I want to impart some of my knowledge to you, to save you the time and frustration of learning by trial and error the way that I did, because I want all of you to get started more quickly than me.

Do you remember a time before you were interested in building things with code? There is a lot of power and value in the ability to make things. You can apply collaboration and code review skills in an unlimited number of situations. GitHub is a very popular place to work on open-source code. Check out GitHub Showcases and Trending to see some of the awesome projects.  

Some benefits of learning collaboration and code review
* If you are a student: being prepared for your studies and career
* If a developer: perhaps you can get a promotion
* In general: you can make cool stuff, make choices that influence product

</td></tr>

<!--
### GitHub Audiences

Organizations
* For-profit (business)
* Not-for-profit

People
* Professional developers
* Hobbyists
* Students

Types of Projects
* Cutting edge
* Novelty
-->


<tr><td width="30%">

![Slide 5]()

</td><td>

### How My Own Journey Began

I want to do a bit of a flashback now. 

I first signed up for GitHub on April 18, 2013. I knew using GitHub was a good idea. But my account sat unused for months. I felt a bit intimidated. I wasn't sure if I fit in and I didn't know how to get started. Later on in this talk, I will debunk some of the myths that I believed at the time. 

</td></tr>


<tr><td width="30%">

![Slide 6]()

</td><td>

### TacoFancy

7 months later, I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker who works in journalism and web development. He had made a really delicious Mexican meal and he and a few other people had decided to start a project on GitHub to share Mexican recipes. 

So I clicked on the link to the repo (definition?) to take a look. 

</td></tr>


<tr><td width="30%">

![Slide 7]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

One sentence in the project README (definition?) made a big impact on me: "Are You New to Github But Want to Contribute?" 

I had been wanting to contribute for months, but wasn't sure how, and now was my chance. I felt it was my destiny to contribute now. 

</td></tr>


<tr><td width="30%">

![Slide 8]()

</td><td>

### My First Pull Request

I didn't quite feel like I knew what I was doing, but I was extremely motivated. I struggled through and submitted my first pull request. As is often characteristic of moments of achievement like this, there was a huge adrenaline rush. 

</td></tr>


<tr><td width="30%">

![Slide 9]()

</td><td>

### It Would Take Almost 3 More Years for Me to Do Code Review

Unfortunately, it would take almost 3 more years for me to begin doing code review. Now that I do it, I wonder, why did it take so long?! It didn't have to be that way. And it would be practical for there to be more maintainers. The number of open-source software users has skyrocketted, but the number of maintainers has not. There is even a concept called the "Bus Factor". If a maintainer got hit by a bus, would there be someone to replace him or her to keep the project going?

</td></tr>


<tr><td width="30%">

![Slide 10]()

</td><td>

### What This Talk Is and Isn’t

<!--
There is a saying, "Don't miss the forest for the trees". It means, don't focus so much on the details that you don't see the larger picture. I think quite often, when people are using Git and GitHub, they are focusing on the details and missing the larger picture. This talk is about the larger picture. 
-->

This talk is about teaching you the underlying logic and essential process between collaboration and code review, so that you can get started as quickly as possible. 

There are many variations to how things can be done in GitHub. This talk is not about teaching you all of those variations. At the end of this talk, you will find links to the official documentation of Git and GitHub where you can find info about variations. 

<!--
I am going to tell you the most typical examples. 
Parts of this process can be reused, for instance, during code review. 
-->

</td></tr>


<tr><td width="30%">

![Slide 11]()

</td><td>

### A Few Notes

* This talk uses GitHub examples, but similar features and workflows could be found in Bitbucket or other services (which some people prefer)
* We will focus on command line, not browser or GUI (such as GitHub Desktop). Can only make full use of git functionality by using command line. (you need to use the command line to do some of the things we are going to do)
* The examples I will be using will focus on public, organizational repos and “Shared Repository Model”, because that is where most of the collaboration and code review are done
* The process is based on GitHub Flow, which is a simple, agile process
* I will identify best practices any time possible
* Some tasks vary by operating system- check tabs at the top of GitHub Help pages for special OS instructions

<!--
Using DjangoCon Example

You will use terminal/command line often with code review.

(<> symbol denotes a placeholder/variable)
Using HTTPS examples
Example- some operating systems do not use dollar signs $ as command line prompts.

https://help.github.com/articles/which-remote-url-should-i-use
SSH URL git@github.com:user/repo.git
HTTPS URL https://github.com/user/repo.git
-->

</td></tr>


<tr><td width="30%">

![Slide 12]()

</td><td>

### Getting Started

* Install Git on your computer and set your email and username
* Create a free [GitHub](https://github.com) account online
* Find and open your computer terminal (a.k.a. command line) on your computer
* The ability to navigate via terminal would be helpful (example: know how to change directory)
* You might also want to have a text editor of your choice installed, to use to edit files

There are a ton of tutorials out there for getting started. I am going to be focused on workflow because there are fewer tutorials out there for what I am going to explain. 

<!--
Text editor recommendations
Bash command list
-->

</td></tr>


<tr><td width="30%">

![Slide 13]()

</td><td>

### Getting Help

* Help via Git, GitHub Help and Guides (links in Useful Resources Section)
* Help via GitHub Keyboard Shortcuts (type "?")
* Help via command line

```bash
$ git help <verb>
$ git <verb> --help
$ man git-<verb>
```

```bash
$ git help clone
$ git clone --help
$ man git-clone
```

<!--
Type q to exit
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Git and GitHub Tour

Git is a version control system that you install on your computer and use via your terminal. GitHub is a web browser dashboard you can use in connection with Git. GitHub is kind of like a social network for developers. You have a profile where you store your code in repositories (a.k.a repos) and you have a newsfeed where you can see the activity of developers you follow. Organizations can have accounts too. 

<!--
What are open-source, Git and GitHub?
At the heart of open source is the idea that by sharing code, we can make better, more reliable software.
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### What Local Environment Looks Like

You can make a copy of a repo (clone) on your computer, make changes, then transfer (push) the changes back to the repo on GitHub. Meanwhile, other users can add their changes. Git and GitHub will record every change to a file and will tell you if there is a conflict. 

<!--
You're going to be transferring file changes back and forth between local Git and GitHub repositories
-->

</td></tr>


<tr><td width="30%">

![Slide 14]()

</td><td>

### Two Types of Accounts

* Organization account
* User account

</td></tr>


<tr><td width="30%">

![Slide 15]()

</td><td>

### Write Permission and Why It Matters

Write Permission is an important concept in GitHub collaboration. 

* Whether you have write permission to a repo determines how you contribute to it
* Having write permission means you can make changes directly inside of the repo 
* Users can't just make changes to any repo. For example, a mission critical software project would not just want anyone to be able to go into the repo and make changes
* There is often a level of trust involved when someone is added to an organization as a maintainer

Some examples of what you can do:
* Push a branch directly to the repo (instead of via fork)
* Edit a file
* Review pull requests

<!--
See write permissions chart for info
-->

</td></tr>


<tr><td width="30%">

![Slide 16]()

</td><td>

### The Two Collaborative Development Models

The question of write permission leads us to Collaborative Development Models. A Collaborative Development Model is a fancy term for the process people go through to contribute to a repo. Which Collaborative Development Model you will use depends on whether you have write permission to the repo you want to contribute to. 

The two Collaborative Development Models: 
* "Shared Repository" Model
* "Fork and Pull" Model

There are two types of accounts and two types of Collaborative Development Models
Conveniently, one collaborative development model typically corresponds to one type of account, and the other collaborative development model typically corresponds to the other type of account

</td></tr>


<tr><td width="30%">

![Slide 17]()

</td><td>

### "Shared Repository"

A “Shared Repository is typically found in an organization account  because it’s where teams of maintainers are working on repos together

</td></tr>


<tr><td width="30%">

![Slide 18]()

</td><td>

### "Fork and Pull"

The “Fork and Pull” Model is typically used in user account repos, because users come across repos they want to contribute to but don’t have write access to and need to fork it to contribute

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Shared Repository Model: User Account Versus Organization

Any repo you come across, whether it be in an organizational account or a user account could be a shared repo or forked repo. For example, a user account owner can give other users write permission to be collaborators on individual repos, which are then "shared repositories", but this is not so common. 

Using an organizational account "Shared Repository" rather than a user account "Shared Repository" for collaboration has some advantages:
* Organizational account owners can create teams and permissions across multiple repos
* Otherwise, the repo "Shared Repository" settings are almost exactly the same

</td></tr>


<tr><td width="30%">

![Slide 19]()

</td><td>

### "Shared Repository" Model Etiquette

Even if you have write permission to a "Shared Repository", just because you can makes changes directly within a repo, without making a pull request, doesn't necessarily mean you should. It is still common to submit a pull request from within the "Shared Repository". If you make a change to the repo without submitting a pull request first, you may be changing code in a live branch. Whether or not you want to do that depends on your level of comfort with the project. It's often still best to have another maintainer review your work through a pull request.

</td></tr>


<tr><td width="30%">

![Slide 20]()

</td><td>

### Example: Forking DjangoCon US Website Repo

The first year that I helped with the DangoCon US website, I was not a maintainer, so I did not have write permission to the DjangoCon US website repo. So, when I wanted to make a change to the repo, I needed to make a copy (fork) the repo to my user account, make the changes, and submit a pull request for the changes to be accepted in the DjangoCon US website repo. This is the "Fork and Pull" Model. 

</td></tr>


<tr><td width="30%">

![Slide 21]()

</td><td>

### Creating a Fork

Two Ways to Fork
* Click the "Fork" button
* Try to edit a file in a repository that you do not have write permission to. GitHub will automatically fork the repo to your user (or organizational) account.

<!--
Forking graphic
-->

</td></tr>


<tr><td width="30%">

![Slide 22]()

</td><td>

### About Forks

When you fork a repo, GitHub creates a copy of the repo, in your user (or organizational) account, with your user name in the URL. The fork will be an exact copy of the original repo at the time it was forked. You will be the only person with write permission to it unless you give collaborator permission to someone else. If you can make any changes to the fork that you want (including adding collaborators), and the original repo will not be affected unless you submit a pull request and a project maintainer pulls your changes into the original repository. When you delete a fork, you are not deleting the original repo. 

<!--
https://help.github.com/articles/fork-a-repo
Most commonly, forks are used to either propose changes to someone else's project/upstream repository or to use someone else's project as a starting point for your own idea.
 -->

</td></tr>


<tr><td width="30%">

![Slide 23]()

</td><td>

### Example: DjangoCon US Website as a "Shared Repository"

<!--
* If you have write permission to a repo (user account or organizational), you can make changes directly within the repo along with other users, this is called the “Shared Repository” Model
-->

</td></tr>


<tr><td width="30%">

![Slide 24]()

</td><td>

### Collaboration and Code Review Best Practice Workflow

In order to be able to increase your level of responsibility, you need to be able to switch between multiple tasks. 
* Keep your code up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 25]()

</td><td>

### Example of a Not-Scalable Workflow

* Fork a repo, make changes directly into the branch you want to change, then submit a pull request. You are then stuck waiting until the pull request is resolved. If you delete the fork and refork the repo, the pull request can still be accepted, but the process becomes more complicated because it's now considered an inactive pull request and it will be more difficult for you to add additional commits to if you are asked to, and for the reviewer to accept.

</td></tr>


<tr><td width="30%">

![Slide 26]()

</td><td>

### How Do We Switch Between Multiple Tasks? 

By using branches

Branches
* Branches are a best practice
* Can be used by any GitHub user
* Give you more freedom

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### About Branches

When you create a repo, you have a default branch named master that contains your initial files. You can make a copy of the master branch and give it a new name and it's a new branch that exists in parallel with the master branch. You can make a change to this new branch and submit a pull request. If the changes are accepted, they can be merged into the master branch. The master branch will be like it was before, except with changes made from the branch.

<!--
You can create unlimited feature branches. Meanwhile, you will want to keep the master and feature branches up-to-date with new merges. 
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Perspective: Submitting a Pull Request

In this example, I am submitting a pull request. It could be either a pull request I am submitting through a fork, when I did not have write access to the DjangoCon US website repo. Or, it could be a pull request that I am submitting through the organizational repo after I became a maintainer. 

<!--
Our perspective is of a person submitting a pull request. The person has cloned a repo (either the organizational repo or a fork) that he or she has write permission to, is going to create a feature branch, make changes to the feature branch, push the branch back to the origin, and submit a pull request for the changes to be merged into the source.
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Remote Origin

A remote is a repo in GitHub that you push or pull code from, and the remote will have a name you will use to refer to it on the command line.

When you clone a repo locally, the repo you cloned from automatically becomes a remote named "origin". "origin" is a default remote. When you push changes to "origin", you will be pushing changes to the repo you cloned from. 

If you cloned from a fork, when you push to "origin", you will be pushing to the fork. If you cloned from an organizational repo, when you push to "origin", you will be pushing to the organizational repo. 

You can then submit a pull request for the new branch in your origin. 

<!--
Will talk later about adding a remote

https://help.github.com/articles/about-remote-repositories
-->

</td></tr>


<tr><td width="30%">

![Slide 30]()

</td><td>

### Bash Commands

Earlier, I said that the ability to navigate via terminal would be helpful (example: know how to change directory). Here are a few very helpful commands.

Go to the home directory

```bash
$ cd
```

Change directory

```bash
$ cd <folder-name>
```

List the folders and files in a directory

```bash
$ ls
```

Move back a directory

```bash
$ cd ..
```

<!--
Bash command list
-->

</td></tr>


<tr><td width="30%">

![Slide 29]()

</td><td>

### Creating and Pushing a Branch, Submitting a Pull Request Overview

The process for creating and pushing a branch is very similar for anyone, regardless of which collaborative development model you are using (organizational repo or forked repo). 

The two main differences are that if you are using the "Fork and Pull" Model:
* If you do not have write permission to the source repo, you need to fork the repo before you use the URL to clone it
* When you submit the pull request, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request.

<!--
Folder/files/text editor

Clone/Download and Push Feature Branch to Repo
-->

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### Commands

Clone (or download) the repo you have write permission to using the repo URL (this repo will be your origin)

```bash
$ git clone <repo-url>
```

Example: clone (or download) an organizational repo (organizational repo will be "origin")

```bash
$ git clone https://github.com/<organization-name>/<repo-name>
```

Example: clone (or download) a user account repo (repo needs to have already been forked to user account, forked repo will be "origin")

```bash
$ git clone https://github.com/<user-name>/<repo-name>
```

A few things that have happened
* There will now be a new folder in the directory you cloned into, by the same name as the repo and filled with the contents of the repo
* The folder will be initialized as a Git repository, with the remote repo named "origin"
* You will be checked out on the default branch (usually master)

<!--
initial copy of the remote repo (using URL) to your local computer

Home directory (command line prompt)
 
https://help.github.com/articles/fetching-a-remote
A remote named origin is created, pointing to the URL you cloned from
-->

Change directory into the folder of the repo you cloned. Folder name will be the repo name.

```bash
$ cd <repo-name>
```

Verify which branch you are checked out on (important if more than one branch)

```bash
$ git branch
```

Create and checkout (switch) to a feature branch, branching off of the branch you intend your changes to be merged into (note how the local files switch to the files of the branch you are checked out on, exactly the same at first, but if you make a change in a branch and then switch back and forth between branches, you can see the difference)

```bash
$ git checkout -b <branch-name>
```

Make your change, then add, commit, create a message (if you don't use -m, a Vim editor will open and you will need to know how to exit)

```bash
$ git add .
$ git commit -m "Your note"
```

Push the new branch to GitHub to your origin (by default, the origin is the repo you cloned from); This can also be used to push additional commits

```bash
$ git push origin <branch-name>
```

There will now be a new branch in the repo that is your origin. The branch will not be affecting anything else. If you never did anything else with it, it would just exist there.

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Alternative Branch Commands

If not working from within the branch you are branching off of, need to specify which branch branching off of (remember, you are branching off the branch you intend your change to be merged into)

```bash
$ git checkout -b <branch-name> <branch-branching-off-of>
```

If the branch already exists, just switch to a branch

```bash
$ git checkout <branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Submit a Pull Request

In the browser, go to the repo you want your pull request to be merged into. There should be a message prompting you to submit a pull request because GitHub will detect your branch. Be forewarned, that if you go to your fork instead, you can accidentally submit a pull request to yourself. 

* Make sure base corresponds to the repo and branch you want to contribute to
* Make sure compare corresponds to your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request 
* Click "Create pull request"

<!--
If you go to the source repo, it will have detected your branch and will suggest that you submit a pull request

base fork, base, head fork, compare
base, compare

branch-name ... "Compare & pull request"
base: master ... compare: branch-name
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Working on Feature Branches and Pull Request Branches

We've established that it's best practice to use branches

Types of branches
* Feature branches (a.k.a. topic branches)
* Pull requests branches

The process for working on feature branches or pull request branches is basically the same (exception: if fetching pull request branch by pull request number)
Anyone with write permission to a feature branch or pull request branch can push additional commits to a feature branch or pull request branch
If a pull request has already been made, the additional commit(s) will be automatically added to the pull request when you push to the branch, up to the point that the pull request is merged
The main difference with a pull request branch is that the reviewer is deciding whether or not to merge, then possibly merging

If you learn to use branches, you will have the fundamentals skills and freedom that will help you to do both collaboration and code review. 

</td></tr>




<tr><td width="30%">

![Slide 00]()

</td><td>

### Remote, Remote Branch, Remote Tracking Branch, and Local Branches

We've already talked about the concept of remotes when we talked about origin

<!--
Hidden folder named .git, storing temporary info from the remote
If you click branches tab, can see a list of the branches
remote branch
remote-tracking branch
local branch

branch from a fork is different though

The remote can be represented by a <remote-name> or a remote URL
-->

</td></tr>


<!--
### How to Add Commits to a Feature Branch or Pull Request

Pushing and pulling via <remote-name>

```bash
$ git pull <remote-name> <branch-name>
$ git push <remote-name> <branch-name>
```

Pushing and pulling via remote URL

```bash
git pull https://github.com/<user-name>/<repo-name> <branch-name>
git push https://github.com/<user-name>/<repo-name> <branch-name>
```
-->


<tr><td width="30%">

![Slide 00]()

</td><td>

### Shared Repo Model Feature or Pull Request Branch

Using origin as an example, because is the most common. Fetch updates to your local .git folder. Create a local branch and insert the contents of the remote branch into it. Merge the master branch into it to keep it up to date. (If the repo was cloned before the pull request)

```bash
$ git fetch origin
$ git checkout -b <local-branch-name> origin/<branch-name>
$ git merge master
```

Push additional commits to organizational pull request

```bash
$ git push origin <branch-name> 
```

Push additional commits to organizational pull request, if local branch name is different than pull request branch name
 
```bash
$ git push origin <local-branch-name>:<remote-branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Forked Repo Model Feature or Pull Request Branch

Create and checkout a new branch (in this case off of the master branch, but could be another). Pull the contents of the remote forked repo branch into it (could be as a feature branch or a pull request branch).

```bash
$ git checkout -b <local-branch-name> master
$ git pull https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo pull request (contributor needs to have given permission, and local branch name and remote branch name need to match)

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo pull request, if local branch name is different than pull request branch name

```bash
$ git push https://github.com/<user-name>/<repo-name> <local-branch-name>:<remote-branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Perspective

We are switching our perspective now. We are now a DjangoCon US website maintainer with write permission to the repo. This is our origin. We are going to review a pull request submitted from within the DjangoCon US website repo. We are also going to be reviewing a pull request submitted from the forked repo. The forked repo is not an origin for us. We would not normally have write permission to the forked repo, but we have been given permission to edit the pull request as a DjangoCon US website maintainer. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Pull Request Review Process

First things first
* If you are a repo maintainer, you will receive a message (by browser or email, based on your notification preferences) to let you know there is a pull request
* Follow the link to the pull request in the repo pull request tab in the browser
* Look over the information about the pull request provided by the contributor

<!--
There will a set of command line instructions for reviewing the pull request locally. The set of instructions will be slightly different depending on whether the pull request was submitted from within the organization as "Shared Repository" Model or from the forked repo (remote branch) as "Fork and Pull" Model.  

- Process is slightly different for "fork and pull" pull request versus "shared repository model" pull request

* click on the files (pull request tab)

Pull request, one file shows all changes

diff Views
* unified view
* split view
* source view
* rich view
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Code Review Options

There are two ways to merge a pull request
* Via browser (click merge button- options are regular, squash, or rebase merge)
* Via command line locally

Simplest scenario
* When you look at the pull request in the browser, you can tell it can be accepted and click merge (for example, if the pull request is fixing a typo) 

Second simplest scenario
* You look at the pull request in the browser. You need to change something, but you can change it in the browser. You edit the file in the browser and click merge (for example, if you fix a typo in the pull request) 

Less simple
* You can't always accept the pull request based on just looking at the code in the browser
* You sometimes need to run the code in the pull request locally to evalute it

After you run the code locally, if you decide a change does need to be made
* You can go back to the browser and click merge

After you run the code locally, if you decide a change needs to be made, there are a few options
* As the contributor to make a change to the pull request
* Push additional commits yourself to the pull request branch


<!--
* you update the pull request branch locally (add, commit, create a message), merge the pull request branch locally via command with the branch it is intended to change, and push to live branch on GitHub

* Fetch pull request branch locally and checkout the branch
fetch the pull request branch to your computer to run the code so that you can evaluate the proposed change. 

* Edit, merge with branch

https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork
* you make change, merge with intended branch and push to origin (follow instructions, live branch/deployed?)

- General process for making a local change, committing, merging and
pushing back to GitHub
- How to keep local code up to date

An example would be if the code for a website has been updated and submitted as a pull request. You can fetch the pull request branch to your computer, checkout the branch, complete any installation process, look at the website in your browser as you run in on a local server, and literally see the change proposed by the pull request. Then decide how to proceed. 

Checkout a pull request locally

* Request a review from a specific person
* Close an issue via commit message by using keyword

Flow chart of possibilities:
-->

</td></tr>




<tr><td width="30%">

![Slide 00]()

</td><td>

### Merge Pull Request Locally and Push to Master Branch

Step 2: Merge the changes and update on GitHub. (Same process no matter where the pull request originated), (merge into the appropriate branch)

```bash
$ git checkout master
$ git merge --no-ff <local-branch-name>
$ git push origin master
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Alternatively, Fetch Individual Pull Request

<!--
Pull updates to the individual pull request into your local branch

```bash
$ git pull origin pull/<pull-request-number>/head:<branch-name>
```

Alternatively, fetch the individual pull request into your folder

```bash
$ git fetch origin pull/<pull-request-number>/head:<branch-name>
```

Example

```bash
$ git fetch origin pull/1/head:patch-1
```

See also, pull request shortcuts
-->

</td></tr>



<tr><td width="30%">

![Slide 39]()

</td><td>

### How to Deal With Merge Conflicts

<!--
Resolve merge conflict:
* resolve in browser
* resolve locally

Advanced
* Resolve a merge conflict in the browser
* Resolve a merge conflict by command line
* Understand rebasing
* Understand update "strategies": fast forward, recursive

Advanced Git
* Git rebase, resolving merge conflicts after a Git rebase

Interactive rebase

Addressing merge conflicts- "competing changes", resolving on GitHub/through command line/text editor
About merge conflicts- Resolve conflicts buttons, can't push until resolved
Resolving a merge conflict on GitHub- only "competing line changes", otherwise do locally
"Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge."
Resolving a merge conflict using the command line- varies by OS, revisit
-->

</td></tr>


<tr><td width="30%">

![Slide 40]()

</td><td>


### Tidy Up

When the pull request is accepted, delete the branch. It's good practice to delete merged or stale branches.  

* Close pull request
* Revert pull request (hopefully not needed)
* Delete local and remote (in browser) feature branch

Delete a branch

```bash
$ git branch -d  <branch-name>
```

Force delete branch

```bash
$ git branch -D  <branch-name>
```

Delete remote branch

```bash
$ git push <remote-name> :<branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Adding an Upstream Remote and Syncing a Fork

The git remote add command takes two arguments:
* A remote name, for example, upstream (you will be using this name in commands to refer to the remote)
* A remote URL, for example, https://github.com/upstream-username/original-repository

Add a remote

```bash
$ git remote add <remote-name> <remote-url>
```

Verify existing remote repository

```bash
$ git remote -v
origin  https://github.com/your-username/your-fork (fetch)
origin  https://github.com/your-username/your-fork (push)
```

Add upstream remote repository that will be synced with the fork

```bash
$ git remote add upstream https://github.com/upstream-username/original-repository.git
```

Verify new upstream remote (can only push to upstream if have write permission)

```bash
$ git remote -v
origin  https://github.com/your-username/your-fork (fetch)
origin  https://github.com/your-username/your-fork (push)
upstream  https://github.com/upstream-username/original-repository (fetch)
upstream  https://github.com/upstream-username/original-repository (push)
```

<!--
If an organizational repo is your origin, because you have write permission, you are fetching from the origin to update your local clone. If you have forked a repo, the organizational repo is your upstream. You will fetch updates from the organizational repo to your local clone, then push the updates to your fork. When the organizational repo changes, the fork is not automatically updated. You need to update the fork, ideally without deleting it (for instance, in case you have unresolved pull requests).

This associates the name origin with the <remote-url>
You should see the URL for your fork as origin, and the URL for the original repository as upstream.
-->

</td></tr>



<tr><td width="30%">

![Slide 00]()

</td><td>

### Syncing Changes

Keep master branch up-to-date

Fetch new branches and commits from the remote repository to local .git folder (add a remote first, if needed), without merging them locally. The branches stored here are called remote-tracking branches.  

```bash
$ git fetch <remote-name>
```

Checkout the branch you will be merging updates into (presumably the branch already exists)

```bash
$ git checkout <branch-name>
```

Merge remote-tracking branch updates with branch you are currently checked out on

```bash
$ git merge <remote-name>/<branch-name>
```

The remote name is often origin or upstream.

Origin example

```bash
$ git fetch origin
$ git checkout master
$ git merge origin/master
```

Upstream example (syncing a fork)

```bash
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
```

Push the changes to your corresponding branch in the forked repository in GitHub

```bash
$ git push origin master
```

Do not pull remote tracking branch updates (defeats the purpose because you already did $ git fetch (updated remote tracking branch with remote changes), which is $ git fetch + $ git merge in one command)

```bash
$ git pull <remote-name>/<branch-name>
```

If pull remote tracking branch updates, and have a problem

```bash
$ git merge --abort
```

Instead, pull directly from the remote repository branch ($ git fetch + $ git merge in one command)

```bash
$ git pull <remote-name> <branch-name>
```

Keep feature branch up-to-date (often merging master into feature branch)

```bash
$ git checkout <feature-branch-name>
$ git merge <branch-name>
```

</td></tr>

<!--
It's good practice to regularly sync your fork with the upstream repository. 
When you make a change on GitHub, the change does not automatically update locally, and vice versa
Deleting a branch in the browser will not delete it in your local repo
The user will make a change in the browser, or clone the repo locally
Browser- opening the website, logging in and making a change directly in the website
When you make a change in the browser, it does not automatically update in your local files
You need to synchronize the changes

you can configure Git to pull changes from the original, or upstream, repository into the local clone of your fork.
When you clone a repository you own, you provide it with a remote URL that tells Git where to fetch and push updates. 

You associate the organizational repo URL with your local clone. 
original repository, you'd add a new remote URL, typically called upstream, to your local Git clone:

git fetch, git merge, git pull

You can always add a new remote and then fetch. https://help.github.com/articles/adding-a-remote
Merging combines your local changes with changes made by others. 

A remote-tracking branch is a branch fetched from a remote repository

Merge a remote-tracking branch with a local branch

For every branch <branch-name> in the remote repository, a corresponding remote-tracking branch 

refs/remotes/<remote-name>/<branch-name>

You can abbreviate the remote-tracking branches as <remote-name>/<branch-name> 

origin/<branch-name> 
upstream/<branch-name>

is created in your local repository. You can usually abbreviate such remote-tracking branch names to origin/foo
remote-tracking branch (i.e., a branch fetched from a remote repository)
non-fast-forward updates were rejected. This means that you must retrieve, or "fetch," the changes

Commits to master will be stored in a local branch, upstream/master. 
Merge the changes from upstream/master into your local master branch. This brings your fork's master branch into sync with the upstream repository, without losing your local changes.
-->

<!--
Merging a remote branch into a local branch

git pull origin <branch-name>

$ git pull origin master
$ git push origin master
-->

<!--
Pull in the changes from the remote branch

$ git pull https://github.com/upstream-username/original-repository <branch-name>
-->




<!--
* repository (called repo for short, a place where a code base is stored)
* source (the original repo someone created, not a fork)
* fork (copy of an entire repo, usually into a user account, but could be into an organization)
* branch (a copy of a code base within a repo, often a "feature branch")

locally (on your own computer)
* local development environment (your computer environment)
* clone (a local copy of a repo)

* remote
* origin (the default name for the remote repository you cloned your code from)
* upstream (source repo (remote) that you pull from in order to push to a fork to keep it up to date/synchronize it)

* git push (use to push commits made on your local branch to a remote repository)
* git fetch (obtain code locally, without merging)
* git merge (merge code)
* git pull (fetch and merge, all in one action)

* pull request (called a pull request because the changes are "pulled into the source repository by the project maintainer")

What is a commit?
Browser (Web)

"the URLs you can use to clone the project onto your computer are available below the repository details:"

Simple Code Review Process

Committing Changes to a Pull Request Branch Created from a Fork

"Above the new content, click Preview changes."

https://help.github.com/articles/pushing-to-a-remote
Tags
https://help.github.com/articles/fetching-a-remote
https://help.github.com/articles/merging-an-upstream-repository-into-your-fork
https://help.github.com/articles/configuring-a-remote-for-a-fork
https://help.github.com/articles/adding-a-remote
https://help.github.com/articles/syncing-a-fork

These commands are very useful when interacting with a remote repository. 
To do this, you'll need to use Git on the command line. 

https://help.github.com/articles/set-up-git/#next-steps-authenticating-with-github-from-git
Step 2: Create a local clone of your fork

To add a new remote, use in the directory your repository is stored at.
Updating organizational clone/reviewing pull requests versus updating fork clone
-->


<tr><td width="30%">

![Slide 00]()

</td><td>

### Browser Versus Local

What your computer screen will look like

</td></tr>

<!--
Examples of How to Do Important Things in Browser versus Locally

Action |Browser | Command Line
:---: | --- | ---
Fork a repo | Can only do in browser | N/A
Create a branch | Open a file and choose "Create a branch new..." | ```$ git checkout -b <branch-name>```
Delete a branch | Branch tab | ```$ git branch -d  <branch-name>```
Create a file | Click "Create new file" button | ```$ touch <file-name>```
Add a file | Click "Upload files" button | ```$ git push origin <remote>```
Commit | Click "Commit changes" button in an open, altered file | ```$ git commit -m  "Your note"```
Open an issue | Can only do in browser | N/A
Open a pull request | Can only do in browser | N/A

Committing changes in browser versus locally
* Can do many things in the browser (example: patch)
* Some changes can be made and committed in the browser, some cannot
* Some things can be done in both browser or command line, some things only by command line locally.

Running code
* Will need to run code locally to view changes, unless dealing with gh-pages and HTML, CSS, JavaScript, or Jekyll

Create, add, rename, move file
Can create, add, rename, move file in browser or from command line (images are an exception)

Branches
Can create a branch in the browser by opening a file and below the commit message field, or through the command line 
Can view/delete branches in the browser by clicking on the branches tab 

branches tab, change default
branch selector menu, click  NUMBER branches to delete
Can delete branches under the branches tab or in the closed pull request page, or by command line
 
Images
Images can be drag and drop/upload, but can't rename or move in browser
* Example: renaming or moving an image file cannot be done in the browser (perhaps drag and drop)

* How/where do you create a user account or organization
* Understand/take tour of the parts of a user account and organization
* Understand how to create teams with permissions
* Access your organizational account and dashboard
* Create an organizational repo
-->




<tr><td width="30%">

![Slide 41]()

</td><td>

### Workflow Decisions

Some projects will involve both a master and develop branch. For example, a mission critical project with a high volume of users is likely to use a develop branch and stage updates before going live.  

If you choose to use a develop branch:
* In addition to the master branch, create the develop branch
* Choose a default branch (can be changed)

<!--
Setting the default branch
"The default branch is considered the base branch in your repository, against which all pull requests and code commits are automatically made, unless you specify a different branch"
The default branch is the base branch and will be master, unless you specify otherwise
Set the default (base branch) under branches tab- against which all pull requests and code commits are automatically made- master branch by default

- [ ] Look at an example of master only versus master/develop, production/staging

* Are you going to have both master and development branches? (master only or master/develop as production/staging)
* default branch? (base against which future pull requests and commits will be made)
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Go Further with Advanced Workflow

Which workflow is "best"? Depends on what you are trying to accomplish. Use the workflow that is right for the projects. They all have pros and cons. Some developers have passionate views about this topic (see comment threads in some posts). 

If you want to know more about advanced workflow:
* Git Flow (basically, the workflow we've been using)
* A Successful Git Branching Model (more advanced)
* A Successful Git Branching Model Considered Harmful (alternative view)
* SemVer
* See also: Atlassian and GitLab docs (you can also find insights in the docs of other software built on top of Git)

* Tags
* Releases

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Organization and Team Setup

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Safeguards Checklist

Setting Up Repo Fail Safes
* Back up the repo (third-party software)
* Protect main branch(es) 
* Enable required reviews of pull requests
* Decide whether to use status checks (external)
* Worst case scenario: How to recover deleted branch
* Sensitive data warning (if made public, consider compromised, immediately remove and change)

</td></tr>


<tr><td width="30%">

![Slide 43]()

</td><td>

### 10X Developers

Important non-coding leadership skills (see 10x results article)
* Keeping docs up to date
* Communication
* People management/mentoring

<!--
https://medium.com/@mikeal/docs-docs-docs-1e06d17fa06f
http://gousios.gr/bibliography/GSB16.html
http://gousios.gr/bibliography/GB15.html
http://opensourcesurvey.org/2017/#insights
http://opensourcesurvey.org/2017/
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Community and Communication Strategy

* What impression you want to give people about your project? Hopefully welcoming, user-friendly. 
* How can you make contributor experience easier/faster/enjoyable (for example, tell people how to contribute)
* Draft community guidelines

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Documentation

<!--
* README.md
* LICENSE (auto-generate, legality of contributions, attribution)
* CODE_OF_CONDUCT.md (auto-generate, choosing from two different Codes of Conduct)
* CONTRIBUTING.md (look at examples for ideas, will generate a message "Please review the guidelines for...")
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Issue and Pull Request Templates

* ISSUE_TEMPLATE
* PULL_REQUEST_TEMPLATE

<!--
* Issues Tab
* Pull Requests Tab
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Forums

* Wikis
* GitHub Pages/Jekyll
* Gists

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Productivity Tips

* Cache your password
* Set up special configs (example: line endings)
* Create saved replies
* Link to specific line number on GitHub

<!--
# Notifications

- [ ] Find the Notifications Overview Page
- [ ] Decide which notifications to receive, whether by browser or email, and which email to receive at

# Conversations

Where They Happen
* Issues
* Pull Requests

Helpers
* GitHub Flavored Markdown 
* @mentions (of people and teams)
* Issue and PR references
* Emojis

Writing and Formatting
* Get to know GitHub Flavored Markdown
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Go For It!

Here are some tips for getting started:

* “Help Wanted” tags, topics/First-timers initiatives
* Look for community-oriented projects and other welcoming projects
* Cherry pick problems or issues that fit your skill level
* Look for triaging (example: node.js website issues)
* Practice your skills and workflow (don't be afraid to delete/start over)
* You can create your own sandbox by making pull requests on your own account or setting up an organization to learn more about options for maintainers

</td></tr>


<!--
Advice of how to get started making pull requests and doing code review
Finding Open Source Projects to Contribute To

* Start where you feel welcome and supported (can evaluate projects using GitHub Open Source Project checklist)

* Search (including advanced search) repositories, code, commits, issues, users, wikis, topics
* Use search syntax "help wanted", "first-timers-only", etc.

* Do a GitHub search such as ["pull requests welcome"](https://github.com/search?utf8=%E2%9C%93&q=pull+requests+welcome)
* [First Timers Only](https://medium.com/@kentcdodds/first-timers-only-78281ea47455#.barzl7cwa)
-->


<tr><td width="30%">

![Slide 00]()

</td><td>

### What If?

<!--
* What if contributors were encouraged to learn code contribution and review at the same time, instead of code review as an end result? More people could take on more responsibility. 
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Debunking Myths

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Thank You :)

Useful Resources: Bitly Link

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>


</table>


## Useful Resources

GitHub and Bitbucket
* [GitHub](https://github.com)
* [Bitbucket](https://bitbucket.org)

Getting Set Up
* [Set Up Git](https://help.github.com/articles/set-up-git)
* [Getting Started Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* [Homebrew Git Formula](http://braumeister.org/formula/git)

Git Official 
* [Git Homepage](https://git-scm.com)
* [Git Doc (Docs and Pro Git Book](https://git-scm.com/doc)
* [Git Documentation](https://git-scm.com/documentation)
* [Git Pro Git Book](https://git-scm.com/book/en/v2)

Glossaries and Cheatsheets
* [GitHub Glossary](https://help.github.com/articles/github-glossary)
* [Git Cheatsheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)
* [GitHub Git Cheatsheet](https://help.github.com/articles/git-cheatsheet)

GitHub Help and Training
* [GitHub Help](https://help.github.com)
* [GitHub Guides](https://guides.github.com)
* [GitHub Training Guides YouTube](https://www.youtube.com/githubguides)

GitHub Try
* [Try Git](https://try.github.io)
* [GitHub Bootcamp](https://help.github.com/categories/bootcamp) 
* [GitHub Hello World Tutorial](https://guides.github.com/activities/hello-world)

GitHub Learning Resources
* [Git and GitHub Learning Resources](https://help.github.com/articles/git-and-github-learning-resources)

GitHub Open Source Guides
* [Open Source Guides](https://opensource.guide)

Writing and Formatting
* [Getting Started with Writing and Formatting on GitHub](https://help.github.com/articles/getting-started-with-writing-and-formatting-on-github)
* [Working with Advanced Formatting](https://help.github.com/articles/working-with-advanced-formatting)

Setting Up and Maintaining Teams
* [Setting Up Teams](https://help.github.com/articles/setting-up-teams)
* [Maintaining Teams](https://help.github.com/articles/maintaining-teams)

Collaborative Development Models and Permission Levels
* [About Collaborative Development Models](https://help.github.com/articles/about-collaborative-development-models)
* [Types of Collaborative Development Models](https://help.github.com/enterprise/2.7/user/articles/types-of-collaborative-development-models)
* [Permission Levels for an Organization](https://help.github.com/articles/permission-levels-for-an-organization)
* [Repository Permission Levels for an Organization](https://help.github.com/articles/repository-permission-levels-for-an-organization)
* [Permission Levels for a User Account Repository](https://help.github.com/articles/permission-levels-for-a-user-account-repository)

<!--
Gitflow 
http://scottchacon.com/2011/08/31/github-flow.html
https://help.github.com/articles/what-is-a-good-git-workflow
https://guides.github.com/introduction/flow
https://help.github.com/articles/about-collaborative-development-models
https://help.github.com/articles/github-flow

Section: releases, working with tags
https://help.github.com/categories/releases
-->

Pull Request Branches Created from a Fork
* [Allowing Changes to a Pull Request Branch Created from a Fork](https://help.github.com/articles/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
* [Committing Changes to a Pull Request Branch Created from a Fork](https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork)

Advanced Collaborative Development Workflow Examples
* Git Flow
* [A Successful Git Branching Model](http://nvie.com/posts/a-successful-git-branching-model) (more advanced)
* [A Successful Git Branching Model Considered Harmful](https://barro.github.io/2016/02/a-succesful-git-branching-model-considered-harmful)
* [SemVer](http://semver.org) (subtopic)

* [Can I Recover Branch After its Deletion in Git?](https://stackoverflow.com/questions/3640764/can-i-recover-branch-after-its-deletion-in-git)

<!--
* [Using Keyboard Shortcuts](https://help.github.com/articles/using-keyboard-shortcuts)

* [Emails (need to be logged in)](https://github.com/settings/emails)
* [Notifications center (need to be logged in)](https://github.com/settings/notifications)

* Browser
* [Desktop App](https://desktop.github.com) (Mac or Windows GUI)
* Command line (recommended, because can do everything with Git)
* [Hub](https://hub.github.com) (makes command line simpler to use)

Pros and Cons
* Some people find GUI (Graphical User Interfaces) such as the Browser or Desktop App to be easier to use


Permission Levels
https://help.github.com/articles/access-permissions-on-github
Owners, members, billing managers, outside collaborators
https://help.github.com/articles/permission-levels-for-an-organization
https://help.github.com/articles/repository-permission-levels-for-an-organization
https://help.github.com/articles/inviting-collaborators-to-a-personal-repository
https://help.github.com/articles/permission-levels-for-a-user-account-repository
https://help.github.com/articles/differences-between-user-and-organization-accounts

* What is [open-source software](https://en.wikipedia.org/wiki/Open-source_software)?

* [A Checklist Before You Contribute](https://opensource.guide/how-to-contribute/#a-checklist-before-you-contribute)

* [Getting to 10x (Results): What Any Developer Can Learn from the Best](https://medium.com/javascript-scene/getting-to-10x-results-what-any-developer-can-learn-from-the-best-54b6c296a5ef)

* [GitHub Pages Basics](https://help.github.com/categories/github-pages-basics)
* [Customizing GitHub Pages](https://help.github.com/categories/customizing-github-pages)
* [Wikis](https://help.github.com/categories/wiki)
* [Gists](https://help.github.com/categories/gists)
* [About READMEs](https://help.github.com/articles/about-readmes)
* [Licensing a Repository](https://help.github.com/articles/licensing-a-repository)
* [Adding a License to a Repository](https://help.github.com/articles/adding-a-license-to-a-repository)
* [Adding a Code of Conduct to Your Project](https://help.github.com/articles/adding-a-code-of-conduct-to-your-project)
-->
