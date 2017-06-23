# Get a Jumpstart on Collaboration and Code Review in GitHub

This is a transcript of a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) will give at [DjangoCon](https://2017.djangocon.us), [PyLadies Remote](http://remote.pyladies.com), and other events.

<!--
* [Original slide deck]()
* [Video recording]()
-->

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016/). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

## Transcript

<table>


<tr><td width="30%">

![Slide 0]()

</td><td>

### Get a Jumpstart on Collaboration and Code Review in GitHub 

By Katherine "Kati" Michel

</td></tr>


<tr><td width="30%">

![Slide 1]()

</td><td>

### Welcome 

I'm thrilled to have the opportunity to talk to you about getting a jumpstart on collaboration and code review in GitHub

</td></tr>


<tr><td width="30%">

![Slide 2]()

</td><td>

### About Me 

* DjangoCon Website Chair
* DEFNA (Django Events Foundation North America) Board Member
* Project Manager
* Web Designer and Developer

</td></tr>


<tr><td width="30%">

![Slide 3]()

</td><td>

### The Journey

Let’s pretend we’re going on a journey. The journey is to learn collaboration and code review. 

</td></tr>


<tr><td width="30%">

![Slide 4]()

</td><td>

### I've Made this Journey Before

When you complete a journey, looking back, sometimes you have learned things. If I were to start my journey over again, I would do things differently from the beginning, knowing what I know now. I want to impart some of my knowledge to you, to save you the time and frustration of learning by trial and error the way that I did, and hopefully you will get started more quickly than me.

</td></tr>


<tr><td width="30%">

![Slide 5]()

</td><td>

### What is the Destination?

Greater autonomy. Collaboration and code review are valuable skills that you can use these skills in an unlimited number of situations. GitHub is a popular place for open-source code. Check out GitHub Showcases and Trending to see some of the awesome projects.  

Some benefits of learning collaboration and code review
* If you are a student: being prepared for your studies and career
* If a developer: perhaps you can get a promotion
* In general: you can make cool stuff, make choices that influence product

</td></tr>


<tr><td width="30%">

![Slide 6]()

</td><td>

### How My Own Journey Began

When I first signed up for GitHub, I felt a bit intimidated. My account sat unused for months.

</td></tr>


<tr><td width="30%">

![Slide 7]()

</td><td>

### TacoFancy: A Taco Recipe Sharing Project on GitHub!

One day, I happened to be looking at Twitter. I saw a tweet from a man named Dan Sinker who works in journalism and web development. He had made a really delicious Mexican meal and he and a few other people had decided to start a project on GitHub to share Mexican recipes. 

</td></tr>


<tr><td width="30%">

![Slide 8]()

</td><td>

### The One Sentence that Motivated Me to Start Using GitHub

I was looking through the Taco Fancy repo and saw one sentence made a big impact on me: "Are You New to Github But Want to Contribute?" I had been secretly wanting to contribute for months, but wasn't sure how, and now was my chance. I really didn't quite know what I was doing, but I was extremely motivated. I struggled through and submitted a pull request. 

</td></tr>


<tr><td width="30%">

![Slide 9]()

</td><td>

### What This Talk Is and Is Not

There are many variations to how things can be done in GitHub. This talk is not about teaching you all of those variations. At the end of this talk, you will find links to the official documentation of Git and GitHub where you can find info about variations. This talk is about teaching you the essential process so that you can get started as quickly as possible. 

</td></tr>


<tr><td width="30%">

![Slide 10]()

</td><td>

### A Few Notes

<!--
* This talk uses [GitHub](https://github.com) examples (GitHub is "the world's leading software development platform"), but similar features and workflows could be found on [Bitbucket](https://bitbucket.org) or other services (which some people prefer)
* I will identify best practices any time possible
* The examples I will be using will focus on public, organizational repos and the "Shared Repository Model" because organizational repos are where most code review happens, but many of the concepts could also be applied to user account collaboration (which I think is lesser known)
* Some tasks vary by operating systems- check tabs at top of some [GitHub Help](https://help.github.com) pages for operating system-specific instructions

(Example: Not all command lines use $)
-->

</td></tr>


<tr><td width="30%">

![Slide 11]()

</td><td>

### Prerequisite Checklist

<!--
I will be focusing on the workflow, but there are tons of tutorials out there for how to get started. There are fewer for what I am going to explain. Example of something that varies by operating system- some operating systems do not use dollar signs as command line prompts.
-->

</td></tr>


<tr><td width="30%">

![Slide 12]()

</td><td>

### Getting Started: Basics

What are Git and GitHub?

High level explanation: You install Git on your computer and create a GitHub account. You can then transfer (clone or push) files back and forth between your computer and GitHub. Git will record every change you commit to the files. 

</td></tr>


<tr><td width="30%">

![Slide 13]()

</td><td>

### Browser Versus Command Line

</td></tr>


<tr><td width="30%">

![Slide 14]()

</td><td>

### Switching Between Multiple Tasks

There is an overall theme to this talk. In order to be able to increase your level of responsibility, you need to be able to switch between multiple tasks. 
* Keep your code up-to-date
* Create one or more features
* Do code review

You can switch between multiple tasks by using "branches". If you learn to use branches, you will have the fundamentals skills and freedom that will help you to do both collaboration and code review. 

</td></tr>


<tr><td width="30%">

![Slide 15]()

</td><td>

### How? By Using Branches!

What is a branch?

</td></tr>


<tr><td width="30%">

![Slide 16]()

</td><td>

### Example of a Not-Scalable Workflow

There are a few problems with this workflow. 

* Fork a repo, make changes directly into the branch you want to change, then submit a pull request. You are then stuck waiting until the pull request is accepted. If you delete the fork, the pull request can still be accepted, but it's considered inactive and you will not be able to add follow-on commits. 

* Clone organizational repo, make changes directly into the branch you want to change, push to branch. Whether or not you should be making changes directly into a live branch depends on your level of comfort with a project. It's often best to have another maintainer review your work through a pull request. 

</td></tr>


<tr><td width="30%">

![Slide 17]()

</td><td>

### Best Practice Workflow

</td></tr>


<tr><td width="30%">

![Slide 18]()

</td><td>

### Two Collaborative Development Models

Collaborative Development Model is a fancy term for how people work together

There are two collaborative development models: 
* “Fork and Pull” Model
* “Shared Repository” Model (usually an organization but could also be a user account repo)

How you contribute to a repo will depend on whether you have read/write access. If you have read/write access to a repo, you can contribute directly to the repo, which is the "Shared Repository" Model. If you do not have read/write access to a repo, you will need to fork the repo to your user account, which is called the "Fork and Pull" Model. 

Note: the advantage of using an organization over user account for "Shared Repository" Model is that an organization can have teams/permissions across projects, not just one owner/repo as is the case with a user account "Shared Repository"

Tip: You have to have read/write access to push directly to a repository

</td></tr>


<tr><td width="30%">

![Slide 19]()

</td><td>

### Read/Write Access

</td></tr>


<tr><td width="30%">

![Slide 20]()

</td><td>

### Read/Write Access Examples

An organization can have teams and permissions; team members working across multiple projects
User account owner can give collaborators read/write access to a repo
Otherwise, shared repository settings are similar

</td></tr>



<tr><td width="30%">

![Slide 21]()

</td><td>

### Branch Process: Virtually the Same

The process for dealing with branches is very similar, regardless of which collaborative development model you are using.

The two main differences are that if you are using the "Fork and Pull" Model:
* You need to fork the repo before you clone it
* You need to check a box when you make the pull request if you want the maintainers to be able to change your pull request

</td></tr>


<tr><td width="30%">

![Slide 22]()

</td><td>

### Branch Process

I want to point out that you can create a branch through the browser, but I will be showing you how to create a branch through terminal/command line, because it's what you will use terminal/command line often with code review.  

</td></tr>


<tr><td width="30%">

![Slide 23]()

</td><td>

### Code Review

If you are a repo maintainer, you will receive a message to let you know there is a pull request (by browser or email, based on your notification preferences). When you go to the pull request, there will a set of instructions for reviewing the pull request locally (on your own computer). The set of instructions will be slightly different depending on whether the pull request was submitted via Forked Repo Model (remote branch) or Shared Repo Model.  

</td></tr>


<tr><td width="30%">

![Slide 24]()

</td><td>

### Forked Repo Model Pull Request

</td></tr>


<tr><td width="30%">

![Slide 25]()

</td><td>

### Shared Repo Model Pull Request

</td></tr>


<tr><td width="30%">

![Slide 26]()

</td><td>

### Tidy Up

* Close pull request
* Revert pull request (if needed)
* Delete feature branch (local and remote)

</td></tr>


<tr><td width="30%">

![Slide 27]()

</td><td>

### Should Your Project Use a Develop Branch?

Some projects will involve both a master and develop branch. For example, a mission critical project with a high volume of users is likely to use a develop branch and staging to gate-keep updates before going live. Use the workflow that is right for the projects. They all have pros and cons. 

If you choose to use a develop branch:
* In addition to the master branch, create the develop branch
* Choose a default branch

If you want to know much more about this, see: A Successful Git Branching Model.

</td></tr>


<tr><td width="30%">

![Slide 28]()

</td><td>

### Go Further with Advanced Workflow

* Git Flow (similar to process I’ve explained)
* A Successful Git Branching Model (more advanced)
* SemVer

</td></tr>


<tr><td width="30%">

![Slide 29]()

</td><td>

### 10X Developers

</td></tr>


<tr><td width="30%">

![Slide 30]()

</td><td>

### Documentation

</td></tr>


<tr><td width="30%">

![Slide 31]()

</td><td>

### Productivity Helpers

</td></tr>


<tr><td width="30%">

![Slide 32]()

</td><td>

### Go For It!

Tips for getting started:

</td></tr>


<tr><td width="30%">

![Slide 33]()

</td><td>

### Debunking Myths

</td></tr>


<tr><td width="30%">

![Slide 34]()

</td><td>

### Useful Resources 

Where to find my slides:

</td></tr>


<tr><td width="30%">

![Slide 35]()

</td><td>

### Thank You :)

Useful Resources: 

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>


</table>

## Useful Resources

Git Official 
* [Git Homepage](https://git-scm.com)
* [Git Doc (Docs and Pro Git Book](https://git-scm.com/doc)
* [Git Documentation](https://git-scm.com/documentation)
* [Git Pro Git Book](https://git-scm.com/book/en/v2)

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
