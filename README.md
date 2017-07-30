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
- [DjangoCon US Website as Example Project](#djangocon-us-website-as-example-project)
- [Goal](#goal)
- [Prerequisites for Getting Started](#prerequisites-for-getting-started)
- [What are Git and GitHub?](#what-are-git-and-github)
- [GitHub: Social Network](#github-social-network)
- [GitHub: Repositories](#github-repositories)
- [Local Development Environment](#local-development-environment)
- [Collaboration and Code Review Best Practice Workflow](#collaboration-and-code-review-best-practice-workflow)
- [Working on a File in GitHub](#working-on-a-file-in-github)
- [Branches](#branches)
- [How to Create a Branch](#how-to-create-a-branch)
- [Overview](#overview)
- [Section 1](#section-1)
- [The Two Collaborative Development Models](#the-two-collaborative-development-models)
- [The Two Types of Accounts](#the-two-types-of-accounts-and-models)
- [Write Permission](#write-permission)
- [Why We Need Write Permission](#why-we-need-write-permission)
- [Write Permission and Collaboration Examples](#write-permission-and-collaboration-examples)
- [How to Fork a Repo](#how-to-fork-a-repo)
- [Forked Repo](#forked-repo)
- [Section 2](#section-2)
- [Fork and Pull Model](#fork-and-pull-model)
- [Shared Repository Model](#shared-repository-model)

<!--
### Local Development Environment
### GitHub Repo Versus Local Directory
### Working on a File Locally
### Local Development Environment
-->

- [New Branch](#new-branch)
- [Submit a Pull Request](#submit-a-pull-request)
- [Section 3](#section-3)

### Perspective: Maintainer

- [Pull Request Review Process](#pull-request-review-process)
- [Checking Out Remote Branches](#checking-out-remote-branches)

- [Tidy Up](#tidy-up)
- [Another Workflow](#another-workflow)
- [Learn More About Workflow](#learn-more-about-workflow)
- [Organization and Team Setup](#organization-and-team-setup)
- [Documentation](#documentation)
- [Safeguards Checklist](#safeguards-checklist)
- [Getting Help](#getting-help)
- [Tips for Getting Started](#tips-for-getting-started)
- [Announcing TacoFancy](#announcing-tacofancy)
- [The One Sentence that Motivated Me to Start Using GitHub](#the-one-sentence-that-motivated-me-to-start-using-github)
- [My First Pull Request](#my-first-pull-request)
- [Thank You](#thank-you)

<!--
- [Local Branch Process](#local-branch-process)

- ["Shared Repository"](#shared-repository)
- ["Fork and Pull" Model](#fork-and-pull-model)

### Pushing and Pulling to Keeping Your Local Clone and GitHub Repo in Sync

### Perspective: Checking Out Remote Branches

### The Difference Between a Feature Branch and a Pull Request Branch
### Fetching from Origin Versus Pulling from a Fork
### Remote, Remote Branch, Remote Tracking Branch, and Local Branches
### Shared Repo Model Feature Branch or Pull Request Branch
### Forked Repo Model Feature Branch or Pull Request Branch

### Merge Pull Request Locally and Push to Master Branch
### Alternatively, Fetch Individual Pull Request
### How to Deal With Merge Conflicts
### Syncing Changes
### Adding an Upstream Remote and Syncing a Fork

### Debunking Myths

- [The Other Way Around](#the-other-way-around)
-->

## Script

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
* DEFNA (Django Events Foundation North America) Board Member
* DjangoCon Europe Website Committee Member
* Project Manager
* Web Designer and Developer

<!--
Engineer
-->

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### Goal

I want to teach you a process that will get you started collaborating and doing code review as quickly as possible. 

I'm going to be showing you a lot of screenshots and diagrams, because I think one of the difficulties of learning Git and GitHub is that it can be difficult to now what the process looks like. I want you to understand what it should look like. 

At the end of my talk, there will be a slide with a link to Useful Resources where you will find documentation and all of the commands I will be showing you today. You will also be able to look at my slides and the video of this online. 

</td></tr>


<!--
<tr><td width="30%">

![Slide 5]()

</td><td>

### Announcing TacoFancy

I want to tell you how I got started with open-source contribution, which is a bit unconventional and might show you that there are many ways to get involved. 

I first signed up for GitHub on April 18, 2013. But my account sat unused for months. I didn't know how to get started.  

7 months later, I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker who works in journalism and web development. He had made a really delicious Mexican meal and he and a few other people had decided to start a project on GitHub to share Mexican recipes. 

So I clicked on the link and went to the project to take a look. 

</td></tr>


<tr><td width="30%">

![Slides 6]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

One sentence in the project information that had a huge impact on me: "Are You New to Github But Want to Contribute?" 

That was me. I had been wanting to contribute for months, but wasn't sure how, and now was my chance. I felt it was my destiny to contribute now. 

</td></tr>


<tr><td width="30%">

![Slides 7]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

Animation

</td></tr>


<tr><td width="30%">

![Slide 8]()

</td><td>

### My First Pull Request

I struggled through, but I was extremely motivated and submitted my first pull request.

</td></tr>


<tr><td width="30%">

![Slide 9]()

</td><td>

### DjangoCon US Website as Example Project

I kept using Git and GitHub and getting better at it. Eventually, I came across the DjangoCon US Website Repo and became a contributor in 2016, then became the Website Chair and maintainer for 2017. 

I am going to use DjangoCon US website as an example throughout this talk. 

<!--
DjangoCon US Website Homepage
DjangoCon US Website Repo
-->

</td></tr>


<tr><td width="30%">

![Slide 10]()

</td><td>

### Prerequisites for Getting Started

* Create a free [GitHub](https://github.com) account online
* Install Git on your computer and set your email and username
* Find and open your computer terminal (a.k.a. command line) on your computer
* The ability to navigate via terminal would be helpful (I will give a few helpful commands in the Useful Resources section)
* You might also want to have a text editor of your choice installed, to use to edit files

You will find documentation for all of these things in the Useful Resources section.

<!--
* By the way, some tasks vary by operating system- check tabs at the top of GitHub Help pages for special OS instructions
* Not all operating systems use the dollar sign as a command line prompt. Just be aware of that
* <variable> is a placeholder for the real thing
-->

</td></tr>


<tr><td width="30%">

![Slide 11]()

</td><td>

### What are Git and GitHub?

GitHub is a website built on the version control software Git. Git is installed in our local development environment and used in the command line of your computer. 

<!--
GitHub Website Landing Page
Git command line- verifying Git is installed and the version
-->

</td></tr>


<tr><td width="30%">

![Slide 12]()

</td><td>

### GitHub: Social Network

GitHub is a social network. You can:
* Make a user account and profile
* Follow people
* Follow their activity in your newsfeed
* Find interesting projects

</td></tr>


<tr><td width="30%">

![Slide 13]()

</td><td>

### GitHub: Repositories

But the really important part of GitHub is that users can store and work on code together in repositories

For example, if you go to the DjangoCon US organization account you will see a list of repos and at the top is the DjangoCon US website repo. If you click on the hyperlink, it will open up the repo and you will see the folders and files filled with the website code and you can look through. 

<!--
DjangoCon US Organization Account List of Repositories
DjangoCon US Website Repo
-->

</td></tr>


<tr><td width="30%">

![Slide 14]()

</td><td>

### GitHub: Repositories

Animation

</td></tr>


<tr><td width="30%">

![Slide 15]()

</td><td>

### GitHub: Repositories

Animation

</td></tr>


<tr><td width="30%">

![Slide 16]()

</td><td>

### Local Development Environment

When we are working on code, we can't do everything in the GitHub website. 

For example, the code in the DjangoCon US website repo is for a website. We cannot run it on GitHub. We sometimes need to make a copy of the code in the local development environment of our computer, install any necessary software, run the code in a local browser on a local server. 

There is where Git is very useful. 

Here is a screenshot of my local development environment. 

* In the background I have GitHub open in the browser
* In front of that, I have my local folder window and my terminal
* I am going to insert the URL (web address) from the browser into a command git clone <url> (copy and paste) and hit enter
* A folder will appear in my home directory by the same name as the GitHub repo and filled with the contents of the repo. Making a copy of a repo locally is called cloning.
* I now have a copy of the code online in the GitHub repo and a copy in my local development environment
* The local folder will also contain another hidden folder named .git that contains the Git configurations.  
* I can make changes to the code, then commit the changes so that Git will record the changes in version control history
* I can push and pull the changes between the GitHub repo and our local development environment to keep them in sync
* Meanwhile, other users can work on the code on their computer and push the changes back to GitHub 
* Occassionally one of us will submit a pull request for our changes to be pulled into the GitHub repo we are working on. 

</td></tr>


<tr><td width="30%">

![Slide 17]()

</td><td>

### Local Development Environment

Animation

</td></tr>


<tr><td width="30%">

![Slide 18]()

</td><td>

### Local Development Environment

Animation

</td></tr>


<tr><td width="30%">

![Slide 19]()

</td><td>

### Collaboration and Code Review Best Practice Workflow

In order to be able to increase your level of responsibility, we need to have the freedom to switch between multiple tasks. 
* You keep your main code branch (master) up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 20]()

</td><td>

### Working on a File in GitHub

When I first started using GitHub, I would go into my own GitHub repo, click on a file, click on the pencil icon to open the file, make a change, and save it. 

This is fine, but imagine if there were multiple people all working on a repo and all of them were going into files and making changes and saving them. It wouldn't be very practical. For instance, how would you give feedback? 

There is a way to make changes that enables you to switch between multiple tasks the way that you need to to collaborate and do code review.

</td></tr>


<tr><td width="30%">

![Slide 21]()

</td><td>

### Working on a File in GitHub

Animation 

</td></tr>


<tr><td width="30%">

![Slide 22]()

</td><td>

### Working on a File in GitHub

Animation 

</td></tr>


<tr><td width="30%">

![Slide 23]()

</td><td>

### Branches

We need to use branches instead. 

Branches
* They are a best practice
* Can be used by any GitHub user

When you create a repo, by default you are working within a branch named master. Say for instance that you want to make a change in the branch, you can make a copy of the entire master branch and give it a different name. Now there are two branches, in the same repo, the master branch and a feature branch. You can create an unlimited number of branches.

At some point, when the feature branch author thinks it's done, a pull request will be submitted and the feature branch will become a pull request branch. If the changes are accepted, they will be merged into the master branch. The master branch will be like before, except with the changes from the branch.  

But both feature branches (a.k.a. topic branches) and pull request branches are examples of remote branches. We can work on them in much the same way. 

</td></tr>

<!--
This could be so that we can add a feature to it, or it could be so that we can look at a change proposed by a pull request and decide how to proceed. 
-->

<tr><td width="30%">

![Slide 24]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 25]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 26]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 27]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### How to Create a Branch

Let's go back to the screenshot of editing a file in GitHub. There is a radial button you can choose to indicate you want to create a new branch. There is also a place to give the branch a new name. When you click to save the changes, they will not save in the current file. Instead, a new branch will be created. 

You can also create and work on branches through the command line in your local development environment, which I will show you later. 

</td></tr>


<tr><td width="30%">

![Slide 29]()

</td><td>

### How to Create a Branch

Animation

</td></tr>


<tr><td width="30%">

![Slide 30]()

</td><td>

### Overview

* Determine which collaboration approach to use (there are two)
* Clone the repo that we have write permission to into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Odds and ends

</td><td>


<tr><td width="30%">

![Slide 31]()

</td><td>

### Section 1

* Determine which collaboration approach to use (there are two)

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### The Two Collaborative Development Models

A Collaborative Development Model is a fancy term for how users contribute to a repo. There are two different ways to contribute. 

The two Collaborative Development Models
* "Shared Repository" Model
* "Fork and Pull" Model

The two different collaborative development models typically correspond to the two different account types

</td></tr>


<tr><td width="30%">

![Slide 33]()

</td><td>

### The Two Types of Accounts

We now know that there are two types of accounts
* Organization accounts such as the DjangoCon organization
* User accounts, such as my own personal account

</td></tr>


<tr><td width="30%">

![Slide 34]()

</td><td>

### Write Permission

We are not talking about "write" permission in the context of English. When a user has write permission to a repo, it means they can make changes directly inside of the repo, probably in a feature branch.

The way that you contribute to a repo depends on whether you have write permission to it. 

</td></tr>


<tr><td width="30%">

![Slide 35]()

</td><td>

### Why We Need Write Permission

Example: DjangoCon US website is a deployed live and has a fairly high volume of traffic. We wouldn't want just anyone to be able to go into the DjangoCon repo and directly make changes. 

</td></tr>


<tr><td width="30%">

![Slide 36]()

</td><td>

### Write Permission and Collaboration Examples

Think about the word "shared". A shared repository is typically found in an organization account where there are teams of maintainers who have write permission to the repos working on them together. 

Example: DjangoCon US Website Repo as a "Shared Repository"

This year I became a maintainer of the DjangoCon US website, so I was given write permission to the DjangoCon US website repo. Along with the other maintainers, I can make changes directly within the DjangoCon US website repo. I no longer need a fork. This is called the "Shared Repository" Model. 

The “Fork and Pull” Model is typically used in user account repos, because users come across repos they want to contribute to but don’t have write permission to it and need to fork it to contribute 

Example: DjangoCon US Website Repo "Fork and Pull" Model

When I first wanted to contribute to the DjangoCon US website, I was not a maintainer, so I did not have write permission to the repo. So I made a copy (or fork) of the DjangoCon US website repo in my user account, made a change, and submitted a pull request to the Django US website repo. When a maintainer approved the pull request, the changes were pulled from the fork into the DjangoCon US website repo. 

This is the "Fork and Pull" Model. 

<!--
In addition to using a fork to propose a change to the original repo, you can also use a fork for the starting point of a new idea of your own (depending on the license). 
-->

</td></tr>


<tr><td width="30%">

![Slide 37]()

</td><td>

### Write Permission and Collaboration Examples

Animation

</td></tr>


<tr><td width="30%">

![Slide 38]()

</td><td>

### Write Permission and Collaboration Examples

Animation

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### How to Fork a Repo

We've gone to the DjangoCon US website repo. 

* Click the "Fork" button
* Try to edit a file in a repository that you do not have write permission to. GitHub will automatically fork the repo to your user (or organizational) account. There will be a message notifying you that it is being forked.. 

</td></tr>


<tr><td width="30%">

![Slide 40]()

</td><td>

### How to Fork a Repo

Animation

</td></tr>



<tr><td width="30%">

![Slide 43]()

</td><td>

### Forked Repo

* The forking message will lead you back to your user account. 
* In the list of repos in your account, you will now see an entry for the fork, which will also tell where it was forked from
* Click on the hyperlink and it will open the repo
* The repo URL will have my user account name in it

You own all of the repos in your user account, including ones you have created and forks. I am the only user with write permission to it unless I give permission to someone else, such as a maintainer, when I am submitting a pull request. The fork is an exact copy of the original repo at the time it was forked. I could make any changes I wanted to the fork, and the original repo will not be affected, including deleting the fork. 

If I submit a pull request and it is accepted, the changes will be pulled into the repo they are intended for.

</td></tr>


<tr><td width="30%">

![Slide 44]()

</td><td>

### Forked Repo

Animation

</td></tr>


<tr><td width="30%">

![Slide 45]()

</td><td>

### Forked Repo

Animation 

</td></tr>


<tr><td width="30%">

![Slide 46]()

</td><td>

### Section 2

* Determine which collaboration approach to use (there are two)
* Clone the repo that we have write permission to into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo

</td></tr>


<tr><td width="30%">

![Slide 47]()

</td><td>

### Fork and Pull Model

* Fork the repo
* Clone the fork, which will now be the remote "origin"
* Make your changes, push the changes back to the fork
* Submit the pull request

Something I want to point out: I mentioned at the beginning of the presentation that when you clone a repo, in the local folder there will be a hidden folder named .git that will contain Git configurations. Git will track some details about the project here, for instance, where the code was cloned from. It will consider the repo the code came from to be a remote repo and will assign the name "origin" to it. We can use the name origin in the command line to refer to the repo. 

<!--
The code in the local clone does not automatically update with the change, and vice versa. 
-->

</td></tr>


<tr><td width="30%">

![Slide 48]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 49]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 50]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 51]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 52]()

</td><td>

### Shared Repository Model

* The fork is not needed
* Clone the shared repository, which will now be the remote "origin"
* Make your changes, push the changes back to the shared repository
* Submit the pull request

<!--
In this situation, our origin is the shared repository
We will talk later about fetching changes
-->

</td></tr>


<tr><td width="30%">

![Slide 53]()

</td><td>

### Shared Repository Model

Animation

</td></tr>


<!--
<tr><td width="30%">

![Slide 00]()

</td><td>

### Minor Differences

The process will be almost the same regardless of whether we are working from a shared repository or fork and pull.

 The two main differences are that if you are using the "Fork and Pull" Model:
* If you do not have write permission to the source repo, you need to fork the repo before you use the URL to clone it
* When you submit the pull request, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request (like I said, maintainers do not automatically have write permission to a fork). 

</td></tr>
-->

<tr><td width="30%">

![Slide 00]()

</td><td>

### Local Development Environment

I am working in my home directory, which you can see from the command prompt. 

Clone (or download) the repo you have write permission to using the repo URL (this repo will be your origin)

```bash
$ git clone <repo-url>
```

Change directory into the folder of the repo you cloned. Folder name will be the repo name.

```bash
$ cd <repo-name>
```

</td></tr>


<tr><td width="30%">

![Slide 55]()

</td><td>

### GitHub Repo Versus Local Directory

You can pull up your GitHub repo and your local folder and compare the files. You can see the corresponding files. The format will be slightly different between one set is being rendered in the browser, and another set are raw files. 

There are some files that you will only see online because they are not needed locally, and vice versa.

</td></tr>


<tr><td width="30%">

![Slide 56]()

</td><td>

### Create a Branch

Verify which branch you are checked out on (important if more than one branch); you will be checkout out on the default branch initially (in this case master, which is the norm)

```bash
$ git branch
```

Create and checkout (switch) to a feature branch, branching off of the branch you intend your changes to be merged into (note how the local files switch to the files of the branch you are checked out on, exactly the same at first, but if you make a change in a branch and then switch back and forth between branches, you can see the difference)

```bash
$ git checkout -b <branch-name>
```

</td></tr>


<tr><td width="30%">

![Slide 56]()

</td><td>

### Working on a File Locally

Make your change, then add, commit, create a message (if you don't use -m, a Vim editor will open and you will need to know how to exit)

```bash
$ git add .
$ git commit -m "Your note"
```

</td></tr>





<tr><td width="30%">

![Slide 57]()

</td><td>

### Pushing a Branch

Push the new branch to GitHub to your origin (by default, the origin is the repo you cloned from that you have write permission to); This can also be used to push additional commits

```bash
$ git push origin <branch-name>
```

There will now be a new branch in the repo that is your origin. If you cloned from the fork, the new branch will be in your fork, if you cloned from the shared repo, the new branch will in the shared repo. 

The branch will not be affecting anything else. If you never did anything else with it, it would just exist there.

</td></tr>



<tr><td width="30%">

![Slide 58]()

</td><td>

### New Branch

<!--
You can toggle back and forth between the branches by clicking on the branches in the branches tab. 
-->

</td></tr>


<tr><td width="30%">

![Slide 59]()

</td><td>

### New Branch

Animation 

</td></tr>


<tr><td width="30%">

![Slide 60]()

</td><td>

### Submit a Pull Request

In the browser, go to the repo you want your pull request to be merged into, in this case, the DjangoCon US website repo. 

There should be a message prompting you to submit a pull request because GitHub will detect your branch and suggest for you to submit a pull request, even if your branch is in a fork. Be forewarned, that if you forked the repo and you go to your fork instead, you can accidentally submit a pull request to yourself. 

* Make sure base corresponds to the repo and branch you want to contribute to
* Make sure compare corresponds to your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, a box will be checked by default giving (upstream) maintainers the ability to edit the pull request 
* Click "Create pull request"

If you are submitting the pull request from within the repo:
* base: master compare:<branch-name>

If you are submitting the pull request a forked repo:
* base fork: django/2017.djangocon.us base: master head fork: katherinemichel/2017.djangocon.us base: <branch-name>

</td></tr>


<tr><td width="30%">

![Slide 61]()

</td><td>

### Submit a Pull Request

</td></tr>


<tr><td width="30%">

![Slide 62]()

</td><td>

### Submit a Pull Request

Animation

</td></tr>


<tr><td width="30%">

![Slide 63]()

</td><td>

### Section 3

* Determine which collaboration approach to use (there are two)
* Clone the repo that we have write permission to into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer

</td></tr>

<!--
Perspective: Reviewing Pull Requests
Point of view: organizational maintainer
Organizational repo is your “origin”
Forked repos branches are remotes
Pull requests are branches
-->

<tr><td width="30%">

![Slide 00]()

</td><td>

### Perspective: Maintainer

We are DjangoCon US website maintainer with write permission to the DjangoCon repo. The DjangoCon US website repo is our origin. 

The forked repo is not an origin for us and we do not have write permission to it, unless we given permission, for example to edit the pull request as a DjangoCon US website maintainer. 

</td></tr>


<tr><td width="30%">

![Slide 64]()

</td><td>

### Pull Request Review Process

* If you are a repo maintainer, you will receive a message (by browser or email, based on your notification preferences) to let you know there is a pull request
* Follow the link to the pull request in the repo pull request tab in the browser
* Look over the information about the pull request provided by the contributor

* There will a set of command line instructions for reviewing the pull request locally. The set of instructions will be slightly different depending on whether the pull request was submitted from within the organization as "Shared Repository" Model or from the forked repo (remote branch) as "Fork and Pull" Model.  

</td></tr>


<tr><td width="30%">

![Slide 43]()

</td><td>

### Checking Out Remote Branches

Even though the command line instructions are for reviewing pull requests locally, they are really for remote branches in general. 

Like we said earlier, anyone with write permission to a feature branch or pull request branch can work on them in much the same way. The main difference is that with a pull request branch, a maintainer will decide whether  to merge the branch into the branch it is intended to be merged with. 

Any person with write permission to a remote branch can fetch it to their local development environment and add commits to it, even if a pull request has already been made. If a pull request has already been made, the additional commits will be automatically added to the pull request when you push the additional commits to the branch, up to the point that the pull request is merged. 

</td></tr>


<tr><td width="30%">

![Slide 44]()

</td><td>

### Remote Tracking Branches

Why are the Instructions Different?

When we are working from within the origin, we can temporarily fetch all of the updates from the origin into the hidden .git folder. When we fetch these updates, they will include branches and commits made directly to the DjangoCon US website, but they will not include branches created through a fork or a pull request branch from a fork, because they come from outside of the origin. 

There are three types of branches:
* remote branch (in a remote repo)
* remote-tracking branch (inside of the hidden .git folder, which stores info)
* local branch

</td></tr>






<tr><td width="30%">

![Slide 00]()

</td><td>

### Pull Request Review Options

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
* You can make the change locally, merge the branch with the branch it is intended to be merged with locally, and push to the branch on GitHub


<!--
https://help.github.com/articles/committing-changes-to-a-pull-request-branch-created-from-a-fork
* push to origin (follow instructions, live branch/deployed?)
An example would be if the code for a website has been updated and submitted as a pull request. You can fetch the pull request branch to your computer. 
Checkout a pull request locally

Merge pull request in browser
Merge pull request locally and push to branch
Ask pull request contributor to update pull request
Update the pull request yourself
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Shared Repo Model Feature Branch or Pull Request Branch

Fetch updates to your local .git folder. Create a local branch and insert the contents of the remote branch into it. Merge the master branch into it to keep it up to date. (If the repo was cloned before the pull request)

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

### Merge Pull Request Locally and Push to Master Branch

Step 2: Merge the changes and update on GitHub. (Same process no matter where the pull request originated), (merge into the appropriate branch)

```bash
$ git checkout master
$ git merge --no-ff <local-branch-name>
$ git push origin master
```

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### How to Deal With Merge Conflicts

Two ways to resolve a merge conflict
* In the browser
* In the local development environment by command line

<!--
* If two people have made different changes to the same part of the code, Git will tell us there is a conflict and one version of the change will need to be chosen

Addressing merge conflicts- "competing changes", resolving on GitHub/through command line/text editor
About merge conflicts- Resolve conflicts buttons, can't push until resolved
Resolving a merge conflict on GitHub- only "competing line changes", otherwise do locally
"Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge."
Resolving a merge conflict using the command line- varies by OS, revisit
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

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

### Syncing Changes

<!--
* The code in the local clone does not automatically update with the change, and vice versa. 

Meanwhile, you keep the master branch and other branches up-to-date by merging in update.  
-->

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

Keep feature branch up-to-date (often merging master into feature branch)

```bash
$ git checkout <feature-branch-name>
$ git merge <branch-name>
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

<!--
Pushing and pulling via <remote-name>
-->

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
Here are the generic commands you can use to push and pull

If you are pushing, you need to have write permission to the branch. The remote can be represented by a <remote-name> or a remote URL
-->

</td></tr>




<!--
When you fork a repo, such as DjangoCon US website repo, when changes are made within that repo, your fork does not automatically update. You could delete your fork and refork it to have a current version, but if you have a pull request submitted, it's not a best practice to delete your fork, because the pull request becomes inactive and it's more difficult for the maintainer and you to work on. So, let's say you have the fork cloned to your local development environment. You cannot push to the DjangoCon US website repo, because you don't have write permission, but you can pull. 

We've talked about how when you clone a repo, Git considers the repo you cloned from to be a remote repo and assigns the name "origin" to it. 
-->

<!--
You can add other remote repos to your local clone and give them a name in order to push and pull from them. We will see an example of this later when we are keeping a fork up-to-date. 

If you clone from the “Shared Repository”, you can just fetch changes directly to your local repo because there is no fork 
If you forked the “Shared Repository" You do this by adding the “Shared Repository” as an upstream, fetching changes, and pushing them to your origin , which is the the fork
-->

<tr><td width="30%">

![Slide 00]()

</td><td>

### Adding an Upstream Remote
### Syncing a Fork

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


<!--
<tr><td width="30%">

![Slide 30]()

</td><td>

### Overview

* Determine which collaboration approach to use (there are two)
* Clone the repo that we have write permission to into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Odds and ends

</td><td>
-->


<tr><td width="30%">

![Slide 00]()

</td><td>

### Learn More About Workflow

* Git Flow (basically, the workflow we've been using)
* A Successful Git Branching Model (more advanced)
* A Successful Git Branching Model Considered Harmful (alternative view)
* SemVer
* See also: Atlassian and GitLab docs (you can also find insights in the docs of other software built on top of Git)

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

![Slide 00]()

</td><td>

### Documentation

Hopefully, you will wnat to create an environment for your project that is welcoming and make the process of contributing fast, easy, and enjoyable. 

<!--
* Draft community guidelines

* README.md
* LICENSE (auto-generate, legality of contributions, attribution)
* CODE_OF_CONDUCT.md (auto-generate, choosing from two different Codes of Conduct)
* CONTRIBUTING.md (look at examples for ideas, will generate a message "Please review the guidelines for...")

### Issue and Pull Request Templates

* ISSUE_TEMPLATE
* PULL_REQUEST_TEMPLATE

* Issues Tab
* Pull Requests Tab
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Tips for getting started

* “Help Wanted” tags, topics/First-timers initiatives
* Look for community-oriented projects and other welcoming projects
* Cherry pick problems or issues that fit your skill level
* Look for triaging (example: node.js website issues)
* Practice your skills and workflow (don't be afraid to delete/start over)
* You can create your own sandbox by making pull requests on your own account or setting up an organization to learn more about options for maintainers

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Go For It!

<!--
Volunteer to help with website
-->

</td></tr>


<tr><td width="30%">

![Slide 00]()

</td><td>

### Thank You

Feel free to contact me by email or on Twitter.

Useful Resources: 
https://git.io/v7LGr

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

<!--
Talk slides and other resources online
-->

</td></tr>


</table>
