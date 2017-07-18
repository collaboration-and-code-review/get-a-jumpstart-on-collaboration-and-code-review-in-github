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

## Table of Contents

- [Get a Jumpstart on Collaboration and Code Review in GitHub](#get-a-jumpstart-on-collaboration-and-code-review-in-github)
- [Welcome](#welcome)
- [About Me](#about-me)
- [About You](#about-you)
- [TacoFancy](#tacofancy)
- [The One Sentence that Motivated Me to Start Using GitHub](#the-one-sentence-that-motivated-me-to-start-using-github)
- [DjangoCon US Website as Example Project](#the-one-sentence-that-motivated-me-to-start-using-github)


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

Thank you for being here. I'm thrilled to have the opportunity to teach you what I've learned you about collaboration and code review in GitHub. 

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### About Me 

A lot of what I'm going to talk to you about, I learned as the DjangoCon US Website Chair

* DjangoCon Website Chair
* DjangoCon Europe Website Committee Member
* DEFNA (Django Events Foundation North America) Board Member
* Project Manager
* Web Designer and Developer

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### About You

This talk is about getting you started collaborating and doing code review as quickly as possible. I want to teach you the essential process and underlying logic, and how they are connected, so you can understand why things are done the way that they are. 

When it comes to Git commands, there are many variations of how things can be done. I'm not going to be going into detail about that. At the end of this talk, there will be a slide with a link to a list of resources which will include the official Git and GitHub documentation. You can learn about all of the variations there. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### TacoFancy

I want to tell you how I got started witih open-source contribution, which is a bit unconventional. 

I first signed up for GitHub on April 18, 2013. But my account sat unused for months. I didn't know how to get started.  

7 months later, I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker who works in journalism and web development. He had made a really delicious Mexican meal and he and a few other people had decided to start a project on GitHub to share Mexican recipes. 

So I clicked on the link and went to the project to take a look. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

One sentence in the project information that had a huge impact on me: "Are You New to Github But Want to Contribute?" 

That was me. I had been wanting to contribute for months, but wasn't sure how, and now was my chance. I felt it was my destiny to contribute now. 

</td></tr>




<tr><td width="30%">

![Slide 9]()

</td><td>

### My First Pull Request

Just like I said earlier, I did not understand what the process was supposed to look like. I didn't quite feel like I knew what I was doing, but I was extremely motivated. I struggled through and submitted my first pull request. As is often characteristic of moments of achievement like this, there was a huge adrenaline rush. 

</td></tr>




<!--
Later on in this talk, I will debunk some of the myths that I believed at the time. 
-->

<!--
I felt a bit intimidated and I wasn't sure if I fit in.

What This Talk Is and Isn’t

Also, I'm hoping that you will understand how commands can be adapted and reused.

I think quite often with Git and GitHub, people learn what they need to know as they need to know it. 

The Journey and Destination
I think people often do not understand the overall process, because they haven't gone that far. 

I like at my process of learning collaboration and code review as being kind of like a journey. When you go on a journey, by the time you are done, you have probably learned something and if you did the journey again, you would do some things differently. If I were to start my journey of learning collaboration and code review over again, knowing what I know now, I would do things differently from the beginning. 

There is a process that supports collaboration and code review and there is a process that doesn't. I want to impart my knowledge to you, to save you the time and frustration of learning by trial and error the way that I did.
-->


<tr><td width="30%">

![Slide 10]()

</td><td>

### It Would Take Almost 3 More Years for Me to Do Code Review

I kept at it. I kept using GitHub and learning about Git. 

Unfortunately, it would take almost 3 more years for me to begin doing code review. Now that I do it, I wonder, why did it take so long?! It didn't have to be that way. The code review process was a mystery to me. I had no idea really how to do it until I asked to do code review for the DjangoCon US website and started doing it. 

The funny thing is, there is actually kind of a shortage of maintainers. There is even a concept called the "Bus Factor". If a maintainer got hit by a bus, would there be someone to replace him or her to keep the project going?

So, it's actually a really positive thing, imo, when someone wants to transition to being a maintainer, because it's filling a need. You would think that it would be good to make becoming a maintainer as obvious and user friendly as possible. But unfortunately, it isn't. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### DjangoCon as Example Project

I am going to use DjangoCon US website as an example throughout this talk. 
* Every example am I going to talk about can be applied to the DjangoCon US website
* They are real examples from my experience

<!--
I hope you've had a chance to take a good look at the DjangoCon website. I'm so proud of what the team has accomplished. It's truly a beautiful website.
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### What are Git and GitHub

Git is a version control system that you install on your computer and use via your terminal. Git by itself is not very user friendly. Some entrepreneurs came along and decided to create a social network for programmers based on GitHub where they can store and work on code in the browser in repositories (a.k.a repos).   

<!--
Git and GitHub Tour
What is open-source?
Definition?
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Getting Started

* Install Git on your computer and set your email and username
* Create a free [GitHub](https://github.com) account online
* Find and open your computer terminal (a.k.a. command line) on your computer
* The ability to navigate via terminal would be helpful (example: know how to change directory, I will give a few helpful commands later)
* You might also want to have a text editor of your choice installed, to use to edit files

There are a ton of tutorials out there for getting started. I am going to be focused on workflow because there are fewer tutorials out there for what I am going to explain. 

<!--
Text editor recommendations
Bash command list
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### A Few Notes

I want to tell you a few things before we get started, so you can understand the context of what we are doing.

* This talk uses GitHub examples, but similar features and workflows could be found in Bitbucket or other services built on Git (which some people prefer)
* We will focus on command line, not browser or GUI (such as GitHub Desktop). Can only make full use of git functionality by using command line. (you need to use the command line to do some of the things we are going to do)
* The examples I will be using will focus on public, organizational repos and “Shared Repository Model”, because that is where most of the collaboration and code review are done
* The process is based on GitHub Flow, which is a simple, agile process
* I will identify best practices any time possible
* Some tasks vary by operating system- check tabs at the top of GitHub Help pages for special OS instructions
* <variable> is a placeholder for the real thing

<!--
Using HTTPS examples, as opposed to SSH HTTPS URL https://github.com/user/repo.git
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Getting Help

* Help via Git, GitHub Help and Guides (links in Useful Resources Section)
* Help via GitHub Keyboard Shortcuts (type "?")
* Help via command line (exit by typing "q")

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

By the way, some operating systems do not use dollar signs $ as command line prompts. Just be aware of that.

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Two Types of Accounts

User account
* A user account is the first type of account create. You have a profile where you store your code in repos and you have a newsfeed where you can see the activity of developers you follow. 

Organization account
* An account where a team of people are working together

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Repository (Repo)

Within user accounts are repos. A repo is a place where a codebase is stored. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Write Permission to a Repo and Why It Matters

Write Permission is an important concept in GitHub collaboration. A person can have write permission to a repo. 

We are not talking about "write" permission in the context of English. When a user has write permission to a repo, it means they can make changes directly inside of the repo. 

Whether you have write permission to a repo determines how you contribute to it (which Collaborative Development Model you use)

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Write Permission Examples

When you create a user account, you are the owner, so you have write permission to all your repos.

Imagine a repo containing a mission critical software project deployed live. It would not be a good idea for just anyone to be able to come along and make changes within that repo. So what happens is that the owner of the organizational account will give write permission to specific users to be maintainers. There is often a level of trust involved. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### The Two Collaborative Development Models

A Collaborative Development Model is a fancy term for the process users go through to contribute to a repo. Which Collaborative Development Model you will use depends on whether you have write permission to the repo you want to contribute to. 

The two Collaborative Development Models: 
* "Fork and Pull" Model
* "Shared Repository" Model

There are two types of accounts and two types of Collaborative Development Models
Conveniently, one collaborative development model typically corresponds to one type of account, and the other collaborative development model typically corresponds to the other type of account

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### "Shared Repository"

A “Shared Repository is typically found in an organization account  because it’s where teams of maintainers are working on repos together. All of the maintainers have write permission to the "Shared Repository" and are therefore able to make changes directly within the repo. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### "Fork and Pull"

The “Fork and Pull” Model is typically used in user account repos, because users come across repos they want to contribute to but don’t have write permission to and need to fork it to contribute. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Example: DjangoCon US Website Repo "Fork and Pull" Model

The first year that I helped with the DangoCon US website, I was not a maintainer, so I did not have write permission to the DjangoCon US website repo. So, when I wanted to make a change to the repo, I needed to fork the repo to my user account, make the changes, and submit a pull request for the changes to be pulled into the DjangoCon US website repo. This is the "Fork and Pull" Model. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Forking the Repo

* Click the "Fork" button
* Try to edit a file in a repository that you do not have write permission to. GitHub will automatically fork the repo to your user (or organizational) account, and notify you that it is forking it. 

<!--
Forking graphic
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Forked the Repo

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### About Forks

So after I forked the repo, I had a copy of the repo in my user account, with my user name in the URL (an organizational account can also fork a repo, but less commmon). The fork would be an exact copy of the original repo at the time it was forked. I owned the fork. I was the only person with write permission to it, unless I would give collaborator permission to someone else. The DjangoCon US website maintainers would not have access unless I gave it to them. I could make any changes to the fork that I wanted, and the original repo will not be affected unless I submitted a pull request and a project maintainer pulled my changes into the DjangoCon US website repository. If I would delete the fork, the original DjangoCon US website repo would not be deleted. 

Forks can be used to propose a change to the original repository, or can be the starting point for a new idea (depending on the license)

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Example: DjangoCon US Website as a "Shared Repository"

The second year that I helped with the DangoCon US website, I became a maintainer, so I was given write permission to the DjangoCon US website repo. I could make changes and submit a pull request within the DjangoCon US website repo, along with the other maintainers. I no longer needed a fork. This is called the "Shared Repository" Model. 

<!--
Some examples of what I can do now:
* Push work (a branch) directly to the repo (instead of via fork)
* Edit a file
* Review pull requests

See write permissions chart for info
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Shared Repository Model: User Account Versus Organization

There is something a bit off topic that I do want to point out. A user account repo can be a "Shared Repository". A user account owner can invite other users to collaborate on a repo that he or she owns. But there are a few advantages to using a organizational repo repo as a "Shared Repository" instead of an user account repo. 

* Organizational account owners can create teams and permissions across multiple repos
* Otherwise, the repo "Shared Repository" settings are almost exactly the same

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### "Shared Repository" Model Etiquette

Even if you have write permission to a "Shared Repository", just because you can makes changes directly within a repo, without making a pull request, doesn't necessarily mean you should. It is still common to submit a pull request from within the "Shared Repository". If you make a change to the repo without submitting a pull request first, you may be changing code in a live branch. Whether or not you want to do that depends on your level of comfort with the project. It's often still best to have another maintainer review your work through a pull request.

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Collaboration and Code Review Best Practice Workflow

In order to be able to increase your level of responsibility, you need to be able to switch between multiple tasks. 
* Keep your code up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 00]()

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
* You can have an unlimited number of branches, so you can do unlimited things

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### About Branches

Whereas a fork is a copy of the entire repo, a branch is a copy of another branch within your repo.

When you create a repo, you have a default branch named master that contains your initial files. You can make a copy of the master branch and give it a new name and it's a new branch that exists in parallel with the master branch. You can make a change to this new branch and submit a pull request. If the changes are accepted, they can be combined (merged) into the master branch. The master branch will be like it was before, except with changes made from the branch.

Meanwhile, you will want to keep the master and feature branches up-to-date by merging in updates. If you want to start working on another feature, you can make another new branch off of the branch it's intended to be merged into.

<!--
Keep main branch(es) up-to-date
Make a copy of the branch you intend to merge your changes into when you want to create a feature
You can have an unlimited number of branches (for example, feature branches or pull request branches)
-->

</td></tr>




<tr><td width="30%">

![Slide 00]()

</td><td>

### Perspective: Submitting a Pull Request

Like I said earlier, you cannot do everything in the browser. You sometimes need to make a copy (clone or download) a repo onto your local computer and work on it locally. 

In this example, I am going to clone a repo from GitHub, create a feature branch locally, make a change to it, push the branch back to the origin repo on GitHub, and submit a pull request for the changes to be merged into the DjangoCon website. 

The process will be almost the same regardless of the situation. 

1. Contributor without write permission forking the repo and cloning the fork
1. Maintainer with write permission cloning the DjangoCo US repo

The two main differences are that if you are using the "Fork and Pull" Model:
* If you do not have write permission to the source repo, you need to fork the repo before you use the URL to clone it
* When you submit the pull request, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request (like I said, maintainers do not automatically have write permission to a fork). 

<!--
Folder/files/text editor
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### What a Local Environment Looks Like

You can also make a copy (clone or download) of a repo on your own computer (local) and work on it. You can transfer (push) changes back and forth between your local computer and your GitHub repositories. And meanwhile other users can work on the code and add their changes too. Git and GitHub will record every change to a file and will tell you if there is a conflict.

<--
You cannot do everything in the browser
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Keeping Your Local Clone and GitHub Repo in Sync

When you clone a repo locally, you now have the code on your computer and in a repo on GitHub. If you make a change to the code locally, the code in the GitHub repo does not automatically update, and vice versa. In order to keep the code in your local clone and in your GitHub repo in sync, you need to push and pull changes between the local clone and the GitHub repo.

GitHub tries to help you with this. When you first clone the repo, the local clone will be connected to the GitHub repo. The GitHub repo is now known as a remote repo and is named "origin" (it's default name). Your local clone will known that it's code came from the origin and you will be able to use the name origin on the command line to push and pull changes between the local clone and GitHub repo to keep them in sync. 

If you cloned from a fork, when you push to "origin", you will be pushing to the fork. If you cloned from an organizational repo, when you push to "origin", you will be pushing to the organizational repo. 

You can also add remotes other than origin to a repo and push and pull from it. We will talk about this later on when we talk about how to update a fork, because when changes are made to the original repo, the fork does not update automatically.

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Pushing and Pulling to Keeping Your Local Clone and GitHub Repo in Sync

Here are the generic commands for pushing and pulling. 

If you are pushing, you need to have write permission to the branch. The remote can be represented by a <remote-name> or a remote URL

Pushing and pulling via <remote-name>

```bash
$ git pull <remote-name> <branch-name>
$ git push <remote-name> <branch-name>
```

Pushing and pulling via remote URL (will come in handy later when we are working with pull request from a fork)

```bash
git pull https://github.com/<user-name>/<repo-name> <branch-name>
git push https://github.com/<user-name>/<repo-name> <branch-name>
```

<!--
fetch it from the remote

```bash
$ git pull <remote-name>
$ git push <remote-name>
```
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
* There will now be a new folder on your computer in the directory you cloned into (probably a home directory, look at command line prompt to know), by the same name as the repo and filled with the contents of the repo
* The folder will be initialized as a Git repository
* You will be checked out on the default branch (usually master)
* The local clone will be connected to the GitHub repository, which is now a remote repository named "origin"

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

<!--
DjangoCon and fork as examples
You can then submit a pull request for the new branch in your origin. 
-->

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

In the browser, go to the repo you want your pull request to be merged into (regardless of whether submitting pull request from within original repo or fork. 

So in my case, I would go to the DjangoCon US website repo. 

There should be a message prompting you to submit a pull request because GitHub will detect your branch and suggest for you to submit a pull request. Be forewarned, that if you go to your fork instead, you can accidentally submit a pull request to yourself. 

* Make sure base corresponds to the repo and branch you want to contribute to
* Make sure compare corresponds to your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request 
* Click "Create pull request"

If you are submitting the pull request from within the repo:
* base: master compare:<branch-name>

If you are submitting the pull request a forked repo:
* base fork: django/2017.djangocon.us base: master head fork: katherinemichel/2017.djangocon.us base: <branch-name>

<!--
DjangoCon example
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Perspective: Checking Out Remote Branches

We are switching our perspective now. We are now working only as DjangoCon US website maintainer with write permission to the DjangoCon repo. The DjangoCon US website repo is our origin. 

We are going to be working on feature branches and reviewing the pull requests we submitted. 

Recap:
1. Pull requests submitted from a branch pushed to the DjangoCon US website repo
2. Pull requests submitted from a forked repo branch

The forked repo is not an origin for us and we do not have write pemrissio to it, unless we given permission, for example to edit the pull request as a DjangoCon US website maintainer. 

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### The Difference Between a Feature Branch and a Pull Request Branch

We've talked about a couple of different types of branches
* Feature branches (a.k.a. topic branches)
* Pull requests branches

When you go to the pull request tab in the browser and look at a pull request, there will a set of command line instructions for reviewing the pull request locally. At the beginning will be a set of instructions for how to fetch the pull request to your computer. Even the instructions are for pull requests, these instructions for fetching the pull request locally work for any remote branch. 

* Anyone with write permission can fetch feature branches and pull request branches, work on them, and push additional commits to them. The process is basically the same (exception: if fetching pull request branch by pull request number).
* If a pull request has already been made, the additional commit(s) will be automatically added to the pull request when you push to the branch, up to the point that the pull request is merged

The main difference between the fetching and working on a feature branch or pull request branch is that with a pull request branch, you eventually decide whether to merge the branch into the branch it is intended to be merged with. 

If you learn to deal with remote branches in general, you will have the fundamentals skills and freedom that will help you to do both collaboration and code review. 

</td></tr>





<tr><td width="30%">

![Slide 00]()

</td><td>

### Fetching from Origin Versus Pulling from a Fork

There is another tricky issue. 

* The way that you fetch or pull a remote branch (feature branch or pull request branch) into your local folder and work on it is different depending on whether the branch was pushed to the shared repository or came from a fork. 

This is why the instructions for reviewing a pull request locally are different depending on whether the pull request was submitted from within the organization as "Shared Repository" Model or from the forked repo (remote branch) as "Fork and Pull" Model. 

Let me explain why. 

<!--
Look for shared repository/original repository references

We are going to be checking out remote branches as a regular maintainer and as a code reviewer. 
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Remote, Remote Branch, Remote Tracking Branch, and Local Branches

When we are working from within the origin, we can fetch all of the updates from the origin to a temporary folder locally called .git. When we fetch these updates, they will include branches and commits made directly to the DjangoCon US website, but they will not include branches created through a fork or a pull request branch from a fork, because they come from outside of the origin. This is why when you go to review a pull request, the instructions are different depending on whether the pull request was submitted from within the origin or from a fork. 

There are three types of branches:
* remote branch
* remote-tracking branch (inside of the hidden .git folder, which stores info)
* local branch

```bash
$ git fetch --prune
$ git branch -a
$ git branch -r
```

<!--
We've already talked about the concept of remotes when we talked about origin.  
-->

</td></tr>




<tr><td width="30%">

![Slide 00]()

</td><td>

### Shared Repo Model Feature Branch or Pull Request Branch

Using origin as an example, because is the most common. Fetch updates to your local .git folder. Create a local branch and insert the contents of the remote branch into it. Merge the master branch into it to keep it up to date. (If the repo was cloned before the pull request)

```bash
$ git fetch origin
$ git checkout -b <local-branch-name> origin/<branch-name>
$ git merge master
```

Push additional commits to organizational feature branch or pull request branch

```bash
$ git push origin <branch-name> 
```

Push additional commits to organizational feature branch or pull request branch, if local branch name is different than pull request branch name
 
```bash
$ git push origin <local-branch-name>:<remote-branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Forked Repo Model Feature Branch or Pull Request Branch

Because it is outside of the origin, it is not fetched in updates. We need to fetch it by its URL. 

Create and checkout a new branch (in this case off of the master branch, but could be another). Pull the contents of the remote forked repo branch into it (could be as a feature branch or a pull request branch).

```bash
$ git checkout -b <local-branch-name> master
$ git pull https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo feature branch or pull request branch (contributor needs to have given permission, and local branch name and remote branch name need to match)

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

Push additional commits to forked repo feature branch or pull request branch, if local branch name is different than pull request branch name

```bash
$ git push https://github.com/<user-name>/<repo-name> <local-branch-name>:<remote-branch-name>
```

</td></tr>



<tr><td width="30%">

![Slide 00]()

</td><td>

### Pull Request Review Process

First things first
* If you are a repo maintainer, you will receive a message (by browser or email, based on your notification preferences) to let you know there is a pull request
* Follow the link to the pull request in the repo pull request tab in the browser
* Look over the information about the pull request provided by the contributor

* There will a set of command line instructions for reviewing the pull request locally. The set of instructions will be slightly different depending on whether the pull request was submitted from within the organization as "Shared Repository" Model or from the forked repo (remote branch) as "Fork and Pull" Model.  

<!--
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

https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork
* you make change, merge with intended branch and push to origin (follow instructions, live branch/deployed?)

- General process for making a local change, committing, merging with branch and
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

<!--
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

Let's go back to the perspective of a person who has cloned a repo locally from a fork.

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

<!--
Do you remember a time before you were interested in building things with code? There is a lot of power and value in the ability to make things. You can apply collaboration and code review skills in an unlimited number of situations. GitHub is a very popular place to work on open-source code. Check out GitHub Showcases and Trending to see some of the awesome projects.  

Some benefits of learning collaboration and code review
* If you are a student: being prepared for your studies and career
* If a developer: perhaps you can get a promotion
* In general: you can make cool stuff, make choices that influence product
-->

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

https://help.github.com/articles/about-remote-repositories
https://help.github.com/articles/fetching-a-remote
https://help.github.com/articles/fork-a-repo

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
