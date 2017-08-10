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
- [Goal](#goal)
- [Announcing TacoFancy](#announcing-tacofancy)
- [The One Sentence that Motivated Me to Start Using GitHub](#the-one-sentence-that-motivated-me-to-start-using-github)
- [My First Pull Request](#my-first-pull-request)
- [DjangoCon US Website as Example Project](#djangocon-us-website-as-example-project)
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
- [The Two Types of Accounts](#the-two-types-of-accounts)
- [Write Permission](#write-permission)
- [Write Permission and Collaboration Examples](#write-permission-and-collaboration-examples)
- [How to Fork a Repo](#how-to-fork-a-repo)
- [Forked Repo](#forked-repo)
- [Section 2](#section-2)
- [Fork and Pull Model](#fork-and-pull-model)
- [Shared Repository Model](#shared-repository-model)
- [Local Dev Environment](#local-dev-environment)
- [Cloning](#cloning)
- [Changing Directory](#changing-directory)
- [GitHub Repo Versus Local Directory](#github-repo-versus-local-directory)
- [Verifying Branch](#verifying-branch)
- [Creating a New Branch](#creating-a-new-branch)
- [Working on a File Locally](#working-on-a-file-locally)
- [Adding and Committing](#adding-and-committing)
- [Pushing](#pushing)
- [New Branch](#new-branch)
- [Submit a Pull Request](#submit-a-pull-request)
- [Section 3](#section-3)
- [Pull Request Review Process](#pull-request-review-process)
- [Pull Request Command Line](#pull-request-command-line)
- [Pull Request Review Options](#pull-request-review-options)
- [Pull Request Branches](#pull-request-branches)
- [Pull Request Review](#pull-request-review)
- [Merging](#merging)
- [Section 4](#section-4)
- [GitHub: Documentation](#github-documentation)
- [Safety Checklist](#safety-checklist)
- [Tips for Getting Started](#tips-for-getting-started)
- [Go for It](#go-for-it)
- [Thank You](#thank-you)


## Script

<table>


<!--
I, you, we
-->

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

Welcome, everyone. I'm Kati Michel. I'm thrilled to have the opportunity to teach you what I've learned as the DjangoCon US Website Chair.

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### About Me 

* DjangoCon Website Chair
* DEFNA (Django Events Foundation North America) Board Member
* Project Manager
* Designer and Developer

<!--
Engineer
-->

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### Goal

I want to teach you a process that will get you started collaborating and doing code review as quickly as possible. 

I'm going to be showing you a lot of screenshots and diagrams, because I want you to understand what the process looks like. 

But don’t worry if you miss anything, because at the end of my talk, there will be a slide with a link to Useful Resources where you will find documentation and all of the commands I will be showing you today. 

My slides and a video of my talk will also be online later.

</td></tr>


<tr><td width="30%">

![Slide 5]()

</td><td>

### Announcing TacoFancy

I want to tell you how I got started with open-source contribution, which I think will show you there are many ways to get involved. 

I first signed up for GitHub in April 2013. But my account sat unused for 7 months. I didn't know how to get started.  

I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker. He had made a really delicious taco meal and decided to start a project on GitHub to share taco recipes. 

So I clicked on the link and went to the project to take a look. 

</td></tr>


<tr><td width="30%">

![Slides 6]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

One sentence in the project information that had a huge impact on me: "Are You New to Github But Want to Contribute?" 

</td></tr>


<tr><td width="30%">

![Slide 7]()

</td><td>

### My First Pull Request

That was me. I became very determined to contribute and submitted my first pull request there.

</td></tr>


<tr><td width="30%">

![Slide 8]()

</td><td>

### DjangoCon US Website as Example Project

I kept using Git and GitHub and getting better at it. I eventually became a DjangoCon US websitie contributor in 2016, then became the Website Chair and maintainer in 2017. 

I am going to use DjangoCon US website as an example throughout this talk. 

<!--
DjangoCon US Website Homepage
DjangoCon US Website Repo
-->

</td></tr>


<!--
* By the way, some tasks vary by operating system- check tabs at the top of GitHub Help pages for special OS instructions
* Not all operating systems use the dollar sign as a command line prompt. Just be aware of that
* <variable> is a placeholder for the real thing
-->


<tr><td width="30%">

![Slide 9]()

</td><td>

### What are Git and GitHub?

GitHub is a website built on the version control software Git.  

<!--
GitHub Website Landing Page
Git command line- verifying Git is installed and the version
-->

</td></tr>


<tr><td width="30%">

![Slide 10]()

</td><td>

### GitHub: Social Network

GitHub is a social network. You can:
* Make a user profile
* Follow people
* Follow their activity in your newsfeed
* Find interesting projects

</td></tr>


<tr><td width="30%">

![Slide 11]()

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

![Slide 12]()

</td><td>

### GitHub: Repositories

Animation

</td></tr>


<tr><td width="30%">

![Slide 13]()

</td><td>

### GitHub: Repositories

Animation

</td></tr>


<tr><td width="30%">

![Slide 14]()

</td><td>

### Local Dev Environment

When we are working on code, we can't do everything in the GitHub website. 

For example, we might want to make a copy of the DjangoCon US website code in the local development environment of our computer, install the necessary software, and run the code in a local browser so that you can add a feature to it, or test a pull request branch.

There is where Git is very useful. Git is installed in our local development environment and used in the command line of your computer. You can use Git to make a snapshot of your project at any point in time and revert back if needed.

Here is a screenshot of my local development environment.

* In the background I have GitHub open in the browser
* In front of that, I have my local folder window and my command line

* I can use the web address (URL) from the GitHub repo in the command line to create a copy of the repo in my local development environment. Making a copy of a repo locally is called cloning.
* I can make changes and push the changes back to GitHub. 
* Meanwhile, other users can do the same thing on their computers.

</td></tr>


<tr><td width="30%">

![Slide 15]()

</td><td>

### Local Dev Environment

Animation

</td></tr>


<tr><td width="30%">

![Slide 16]()

</td><td>

### Local Dev Environment

Animation

</td></tr>


<tr><td width="30%">

![Slide 17]()

</td><td>

### Collaboration and Code Review Best Practice Workflow

There is a concept that I think is very important.

In order to be able to increase your level of responsibility, we need to have the freedom to switch between multiple tasks. 
* You keep your main code branch (master) up-to-date
* Create one or more features
* Do code review

</td></tr>


<tr><td width="30%">

![Slide 18]()

</td><td>

### Working on a File in GitHub

When I first started using GitHub, I would go into my own GitHub repo, click on a file, click on the pencil icon to open the file, make a change, and save it. 

This is fine, but imagine if there were multiple people all working on a repo and all of them were going into files and making changes and saving them. It wouldn't be very practical. For instance, how would you give feedback? 

There is a way to make changes that enables you to switch between multiple tasks the way that you need to to collaborate and do code review.

</td></tr>


<tr><td width="30%">

![Slide 19]()

</td><td>

### Branches

We need to use branches instead. 

Branches
* They are a best practice
* Can be used by any GitHub user

When you create a repo, by default you are working within a branch named master. Say for instance that you want to make a change in the branch, you can make a copy of the entire master branch and give it a different name. Now there are two branches, in the same repo, the master branch and a feature branch. You can create an unlimited number of branches and you can switch in between them to work on them.

At some point, when the feature branch author thinks it's done, a pull request will be submitted and the feature branch will become a pull request branch. If the changes are accepted, they will be merged into the master branch. The master branch will be like before, except with the changes from the branch.  

But both feature branches (a.k.a. topic branches) and pull request branches are examples of branches. We can work on them in much the same way. 

</td></tr>


<tr><td width="30%">

![Slide 20]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 21]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 22]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 23]()

</td><td>

### Branches

Animation

</td></tr>


<tr><td width="30%">

![Slide 24]()

</td><td>

### How to Create a Branch

Let's go back to the screenshot of editing a file in GitHub. There is a radial button you can choose to indicate you want to create a new branch. There is also a place to give the branch a new name. When you click to save the changes, they will not save in the current file. Instead, a new branch will be created. 

You can also create and work on branches through the command line in your local development environment, which I will show you later. 

</td></tr>


<tr><td width="30%">

![Slide 25]()

</td><td>

### How to Create a Branch

Animation

</td></tr>


<tr><td width="30%">

![Slide 26]()

</td><td>

### Overview

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional info

</td><td>


<tr><td width="30%">

![Slide 27]()

</td><td>

### Section 1

* Determine which collaboration approach to use (there are two)

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### The Two Collaborative Development Models

A Collaborative Development Model is a fancy term for how users contribute to a repo. There are two different models. 

The two Collaborative Development Models
* "Shared Repository" Model
* "Fork and Pull" Model

The two different models typically correspond to the two different account types and which model you uses depends on whether you have write permission to the repo. 

</td></tr>


<tr><td width="30%">

![Slide 29]()

</td><td>

### The Two Types of Accounts

There are two types of accounts
* Organization accounts such as the DjangoCon organization
* User accounts, such as my own personal account

</td></tr>


<tr><td width="30%">

![Slide 30]()

</td><td>

### Write Permission

When a user has write permission to a repo, it means they can make changes directly inside of the repo.

</td></tr>


<tr><td width="30%">

![Slide 31]()

</td><td>

### Write Permission and Collaboration Examples

First, we’ll look at the “Shared Repository” Model. A shared repository is typically found in an organization account, which makes sense when you think about the word shared.
* For example, this year I became a maintainer of the DjangoCon US website, so I was given write permission to the DjangoCon US website repo, which is a “Shared Repository”. Along with the other maintainers I work with who have write permission, I can make changes directly within the DjangoCon US website repo.

The “Fork and Pull” Model is typically used in user account repos. For example, when I first came across the DjangoCon US website repo, I wanted to contribute, but I was not a maintainer, so I didn't have write permission. So I made a copy (a.k.a. fork) of the DjangoCon US website repo in my user account, which I have write permission to, made a change, and submitted a pull request to the Django US website repo. 

<!--
When a maintainer approved the pull request, the changes were pulled from the fork into the DjangoCon US website repo.
If I submit a pull request and it is accepted, the changes will be pulled into the repo they are intended for.
* Occassionally one of us will submit a pull request for our changes to be pulled into the GitHub repo we are working on. 
-->

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### Write Permission and Collaboration Examples

Animation

</td></tr>


<tr><td width="30%">

![Slide 33]()

</td><td>

### How to Fork a Repo

We've gone to the DjangoCon US website repo. 

* Click the "Fork" button
* Try to edit a file in a repository that you do not have write permission to. GitHub will automatically fork the repo to your user account. There will be a message notifying you that it is being forked.

</td></tr>


<tr><td width="30%">

![Slide 34]()

</td><td>

### How to Fork a Repo

Animation

</td></tr>


<tr><td width="30%">

![Slide 35]()

</td><td>

### Forked Repo

* The forking message will lead you back to your user account. 
* In the list of repos in your account, you will now see an entry for the fork, which will also tell where it was forked from
* Click on the hyperlink and it will open the repo
* The repo URL will have my user account name in it

The fork is an exact copy of the original repo at the time it was forked. I could make any changes I wanted to the fork, including deleting it, and the original repo will not be affected. 

</td></tr>


<tr><td width="30%">

![Slide 36]()

</td><td>

### Forked Repo

Animation

</td></tr>


<tr><td width="30%">

![Slide 37]()

</td><td>

### Forked Repo

Animation 

</td></tr>


<tr><td width="30%">

![Slide 38]()

</td><td>

### Section 2

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo

</td></tr>


<tr><td width="30%">

![Slide 39]()

</td><td>

### Fork and Pull Model

I've made a couple of diagrams that I hope will give you an idea of what the process is for working locally for each collaborative development model. 

* Fork the repo
* Clone the fork. 

Git will track some details about the project, for instance, where we cloned our code from. In relation to the clone, the GitHub repo we cloned from is now a remote repo and Git will assign the name "origin" to it. We can use the name origin in the command line to refer to the repo so we can push and pull changes back and forth between the local development environment and the GitHub repo.

* Make our changes, push the changes back to the fork
* Submit the pull request

<!--
The GitHub repo does not automatically update when we make a change locally and vice versa. We have to update it.
-->

</td></tr>


<tr><td width="30%">

![Slide 40]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 41]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 42]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 43]()

</td><td>

### Fork and Pull Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 44]()

</td><td>

### Shared Repository Model

Here's what it looks like when we use the "Shared Repository" Model

* The fork is not needed, because we have write permission
* Clone the shared repository. The shared repository will now be the remote "origin"
* Make our changes, push the changes back to the shared repository
* Submit the pull request

</td></tr>


<tr><td width="30%">

![Slide 45]()

</td><td>

### Shared Repository Model

Animation

</td></tr>


<tr><td width="30%">

![Slide 46]()

</td><td>

### Shared Repository Model

Animation

</td></tr>





<tr><td width="30%">

![Slide 47]()

</td><td>

### Local Development Environment

What I'm going to show you now is a generic process that you can use for a shared repository or a fork. You will clone the repo you have write permission to.

Let's go back to the screenshot of my local development environment. 

* I am working in my home directory. The name of home directory is at the top of the command line, and in front of the prompt. The reason why this matters is because the repo will be cloned into the directory we are working in.

* I am going to type the command $ git clone into the command line and copy and paste the URL from the browser of either the shared repo or fork, then hit enter. 

* A folder will appear in my home directory by the same name as the GitHub repo (2017.djangocon.us) and filled with the contents of the repo.  
* I now have a copy of the code online in the GitHub repo and a copy in my local development environment. 

* I will now change directory into the folder so that I can work there by typing cd 2017.djangocon.us, which is the folder name.

* I've clicked on the folder in the folder window so that I can see the contents visually. But I can also see I am working from within the folder in my command line because the name of the folder is at the top of the command line and in front of the prompt. 

* You can pull up your GitHub repo and your local folder and compare the files. You can see the corresponding files. The format will be slightly different between one set is being rendered in the browser, and another set are raw files. 

* Use the command $ git branch to verify which branch you are checked out on; initially, you will be checkout out on the default branch (in this case master)

* Create and checkout (switch) to a feature branch. We are calling this feature branch example-branch. We want to branch off of the branch we intend our changes to be merged into (note how the local files switch to the files of the branch you are checked out on, exactly the same at first, because a copy, but if you make a change in a branch and then switch back and forth between branches, you can see the difference)

<!--
* We created and checked-out to a branch by the name of example-branch
-->

* Open a file in the text editor. Make your change and save it.

* Add and commit our change to git version control, create a message "Creating branch and updating"

* Push the new branch named example-branch to GitHub to your origin (the repo you cloned from that you have write permission to)


<!--
* I can push and pull the changes between the GitHub repo and our local development environment to keep them in sync
-->

```bash
$ git clone <repo-url>
$ cd <repo-name>
$ git branch
$ git checkout -b <branch-name>
$ git add .
$ git commit -m "Your note"
$ git push origin <branch-name>
```

```bash
$ git clone https://github.com/djangocon/2017.djangocon.us
or
$ git clone https://github.com/KatherineMichel/2017.djangocon.us
$ cd 2017.djangocon.us
$ git branch
$ git checkout -b example-branch
$ git add .
$ git commit -m "Creating branch and updating"
$ git push origin example-branch
```

<!--
Take the time to make sure your changes work
Leave a clear commit message
-->

</td></tr>




<tr><td width="30%">

![Slide 48]()

</td><td>

### Cloning

Animation

</td></tr>


<tr><td width="30%">

![Slide 49]()

</td><td>

### Cloning

Animation

</td></tr>


<tr><td width="30%">

![Slide 50]()

</td><td>

### Changing Directory

Animation

</td></tr>


<tr><td width="30%">

![Slide 51]()

</td><td>

### Changing Directory

Animation

</td></tr>


<tr><td width="30%">

![Slide 52]()

</td><td>

### GitHub Repo Versus Local Directory

Animation

</td></tr>


<tr><td width="30%">

![Slide 53]()

</td><td>

### Verifying Branch

Animation

</td></tr>


<tr><td width="30%">

![Slide 54]()

</td><td>

### Creating a New Branch

Animation

</td></tr>


<tr><td width="30%">

![Slide 55]()

</td><td>

### Working on a File Locally

Animation

</td></tr>


<tr><td width="30%">

![Slide 56]()

</td><td>

### Adding and Committing

Animation

</td></tr>


<tr><td width="30%">

![Slide 57]()

</td><td>

### Pushing

Animation

</td></tr>


<tr><td width="30%">

![Slide 58]()

</td><td>

### New Branch

There will now be a new branch in the repo that is your origin and a message telling you it's there. If you click on the branch tab you can choose the name of the branch to switch to the new branch. You can toggle back and forth between the branches by clicking on the branches in the branches tab. 

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

Go to the repo you want your pull request to be merged into, in this case, the DjangoCon US website repo. There will also be a message here telling you about the branch and suggesting that you submit a pull request, even if the branch is in a fork, because GitHub will detect it. Click on the "Compare & pull request" button. 

* Make sure that the base branch is the branch you want your change to be merged into
* Make sure compare branch is your branch
* Create a pull request title and perhaps a description
* If the pull request is via a forked repo, a box will be checked by default giving maintainers the ability to edit the pull request 
* Double check your changes
* Click "Create pull request"

</td></tr>


<tr><td width="30%">

![Slide 61]()

</td><td>

### Submit a Pull Request

Animation

</td></tr>


<tr><td width="30%">

![Slide 62]()

</td><td>

### Section 3

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer

</td></tr>


<tr><td width="30%">

![Slide 63]()

</td><td>

### Pull Request Review Process

* When a pull request is submitted repo maintainers will receive a notification by browser or email to let them know there is a pull request
* Follow the link to the pull request tab in the browser
* Look over the information about the pull request. You can see the title and description and click on the “Files changed” link to see all of the changes that were made. 

Underneath that will be info about how to merge the pull request. 
* There will be a merge button that you can click to merge in the browser
* Or there will be a link that says “command line instructions” 

</td></tr>


<tr><td width="30%">

![Slide 64]()

</td><td>

### Pull Request Review Process

Animation

</td></tr>


<tr><td width="30%">

![Slide 65]()

</td><td>

### Pull Request Command Line

When you click on that link, it will open up a set of instructions for how to review and merge the pull request in your local development environment. The instructions will be different depending on whether the pull request was submitted from within the shared repository or from a forked repo.  
I will go over that in a minute. 

I will go over that in a minute. 

</td></tr>


<tr><td width="30%">

![Slide 66]()

</td><td>

### Pull Request Review Options

But first, let's go over the options for what you can do when you review a pull request.

The first two options involve clicking the merge button in GitHub without running the code locally
* You look at the pull request changes, you can tell they can be accepted and click merge  
* You look at the pull request changes. Something needs to be changed, but you can change it in GitHub. So you edit the pull request file in the browser, similarly to how we edited a file earlier, and click merge.

</td></tr>


<tr><td width="30%">

![Slide 67]()

</td><td>

### Pull Request Review Options

The other options involve fetching the pull request into your locally development environment and running the code there. 

If a change does not need to be made, you can
* Go back to the browser and click merge

If a change needs to be made, you can
* Ask the pull request author to make a change to the pull request
* Make the change locally yourself and push additional commits to the pull request branch on GitHub
* Make the change locally yourself, merge the branch with the branch it is intended to be merged with locally, and push to the branch on GitHub

</td></tr>


<tr><td width="30%">

![Slide 68]()

</td><td>

### Pull Request Branches

We are DjangoCon website maintainers and the DjangoCon US website repo is our origin. 

This is why the pull request instructions are different. 

As a DjangoCon US website maintainer, we are able to fetch updates made to the DjangoCon US website repo into a hidden folder named .git in our local development environment. These updates will include branches made directly to the DjangoCon US website repo, but they will not include branches made through a fork, because they come from outside of the origin. 

Branches made through a fork need to be pulled individually into our local development environment.

</td></tr>


<tr><td width="30%">

![Slide 69]()

</td><td>

### Pull Request Review

The instructions on this slide can actually be used by any maintainer to work on any branch they have write permission to.  
If a pull request has already been made, the additional commits will be automatically added to the pull request, up to the point that the pull request is merged.

For a shared repository pull request, we use the command $ git fetch origin to fetch the updates into the .git folder. We create and checkout to a new local branch, which we give a name to, and we insert the pull request branch contents from the .git folder into the new local branch by referring to the branch as origin/<branch-name>. We can merge master to make sure the branch is up-to-date. If we make a change, we can push additional commits to the branch on GitHub. 

For a pull request submitted through a fork, we create a new branch off master and pull in the contents of the pull request branch from the fork. If we make a change, we can also push additional commits if we have been given permission to edit the pull request. 

```bash
$ git fetch origin
$ git checkout -b <local-branch-name> origin/<branch-name>
$ git merge master
```

```bash
$ git push origin <branch-name> 
```

```bash
$ git checkout -b <local-branch-name> master
$ git pull https://github.com/<user-name>/<repo-name> <branch-name>
```

```bash
$ git push https://github.com/<user-name>/<repo-name> <branch-name>
```

<!--
Push after changes are made and committed
-->

</td></tr>


<tr><td width="30%">

![Slide 70]()

</td><td>

### Merging

This piece of code is for merging a pull request locally and pushing to the master branch.  

You are checking out to the master branch, merging the feature branch into the master branch, then pushing the change to the live master branch on GitHub. 

```bash
$ git checkout master
$ git merge --no-ff <local-branch-name>
$ git push origin master
```

</td></tr>


<tr><td width="30%">

![Slide 71]()

</td><td>

### Section 4

* Determine which collaboration approach to use (there are two)
* Clone a repo into our local development environment, create a feature branch, make a change, push the branch to the GitHub repo we cloned from, and submit a pull request to DjangoCon US Website repo
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Additional info

</td><td>





<tr><td width="30%">

![Slide 72]()

</td><td>

### GitHub: Documentation

Hopefully, you will want to create a welcoming environment for your project. Your documentation might inspire someone else to contribute to a project the way that I was inspired to contribute to TacoFancy. You can do this by creating several different pieces of documentation.

GitHub can help you to generate a LICENSE and CODE_OF_CONDUCT.md based on commonly used licenses and codes
* LICENSE- tells you the legal terms under which you can contribute and use the code
* CODE_OF_CONDUCT.md- a set of rules outlining the expectations and responsibilities of contributors 
* README.md- gives general project information
* CONTRIBUTING.md- gives info about contributing. When a contributing document is present, when someone creates an issue, they will see a message prompting them to read the contributing document.

</td></tr>


<tr><td width="30%">

![Slide 73]()

</td><td>

### Safety Checklist

You might want to go to the Settings area of a repo and click the Branches tab
* Protect branch the main branch so it can’t be deleted (for example, your master branch)
* Enable required reviews of pull requests, for example, a review has to be done before a pull request can be merged

</td></tr>



<tr><td width="30%">

![Slide 74]()

</td><td>

### Tips for Getting Started

In the Useful Resources Section there is an excellent checklist for evaluating a project and I recommend that you take a look because it's very comprehensive.



* “Help Wanted” tags, topics/First-timers initiatives
* Look for community-oriented projects and other welcoming projects
* Look for projects where triaging happens and pick issues or pull requests that fit your skill level
* Practice your skills and workflow (don't be afraid to delete/start over)
* You can create your own sandbox by making pull requests on your own account or setting up an organization to learn more about options for maintainers

</td></tr>



<tr><td width="30%">

![Slide 75]()

</td><td>

### Go For It!

* By the way, if you are interested in contributing to the DjangoCon US website next year, let us know. We have a diverse group of contributors of all skill levels and we are always looking for more contributors. 

</td></tr>


<tr><td width="30%">

![Slide 76]()

</td><td>

### Thank You

Feel free to contact me.

Useful Resources: 
https://git.io/v7LGr

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>


</table>
