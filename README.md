# Get a Jumpstart on Collaboration and Code Review in GitHub- PyLadies Southwest Florida

# Table of Contents

- [About](#about)
- [GitHub and Git Installation Instructions](#github-and-git-installation-instructions)
- [Important Hacktoberfest Links](#important-hacktoberfest-links)
- [Slides and Script Table of Contents](#slides-and-script-table-of-contents)
- [Slides and Script](#slides-and-script)
- [Useful Resources](#useful-resources)
    - [Links](#links)    
- [Attribution](#attribution)
- [Contact Kati](#contact-kati)
- [Copyright](#copyright)

<hr>

## About

Slides and script for a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) gave to PyLadies Southwest Florida, PyLadies Miami, SWFL Coders, SFWL Data, and FGCU SEC Thursday, September 24, 2020 at 6:00 p.m. CST via Zoom.
 
Meetup Page
* ["Get a Jumpstart on Collaboration and Code Review in GitHub"](https://www.meetup.com/PyLadies-SWFL/events/273309212/)

Slide Deck and Video Recording
* [Original slide deck](https://docs.google.com/presentation/d/17UG5OwojhiHYAaFjVJLncDdqMGHQAjk_W0rLoEgIp8Q/edit?usp=sharing)
* Video recording

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## GitHub and Git Installation Instructions

* [GitHub Homepage (for user account signup)](https://github.com)
* [Git Downloads (based on your operating system)](https://git-scm.com/downloads)
* [Getting Started Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
* [Homebrew Git Formula (for Mac users who use Homebrew)](https://formulae.brew.sh/formula/git)
* [Setting Your Username in Git](https://docs.github.com/en/github/using-git/setting-your-username-in-git)
* [Setting Your Email Address in Git](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/setting-your-commit-email-address)

### A few helpful commands

Verify that Git is installed by typing into your command line

```bash
$ git --version
```

Verify that your username is set by typing into your command line

```bash
$ git config --global user.name
```

Verify that your email is set by typing into your command line

```bash
$ git config --global user.email
```

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Important Hacktoberfest Links

* [Hacktoberfest Website](https://hacktoberfest.digitalocean.com)
* ["Browse all participating Hacktoberfest projects on GitHub"](https://github.com/search?q=label:hacktoberfest+state:open+type:issue)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script Table of Contents

- [Get a Jumpstart on Collaboration and Code Review in GitHub](#get-a-jumpstart-on-collaboration-and-code-review-in-github)
- [Welcome](#welcome)
- [About Me](#about-me)
- [Talk Goal](#talk-goal)
- [Good News](#good-news)
- [More Good News](#more-good-news)
- [More Good News- Hacktoberfest](#more-good-news-hacktoberfest)
- [Announcing TacoFancy](#announcing-tacofancy)
- [One Life Changing Question](#one-life-changing-question)
- [My First Pull Request](#my-first-pull-request)
- [DjangoCon US Website as Example Project](#djangocon-us-website-as-example-project)
- [Prerequisites for Getting Started](#prerequisites-for-getting-started)
- [Housekeeping](#housekeeping)
- [What are Git and GitHub?](#what-are-git-and-github)
- [Social Network](#social-network)
- [Repositories](#repositories)
- [Local Development Environment Example](#local-development-environment-example)
- [Workflow Overview](#workflow-overview)
- [The Two Collaborative Development Models](#the-two-collaborative-development-models)
- [The Two Types of Accounts](#the-two-types-of-accounts)
- [Write Permission](#write-permission)
- [Examples of What Write Permission Will Allow You to Do](#examples-of-what-write-permission-will-allow-you-to-do)
- [Why We Need Write Permission](#why-we-need-write-permission)
- [Write Permission and Collaboration Examples](#write-permission-and-collaboration-examples)
- [How to Fork a Repo](#how-to-fork-a-repo)
- [Forked Repo](#forked-repo)
- [Workflow Overview](#workflow-overview)
- [Collaboration and Code Review Best Practice Workflow Using Branches](#collaboration-and-code-review-best-practice-workflow-using-branches)
- [Working on a File in GitHub](#working-on-a-file-in-github)
- [Reasons for Using Branches](#reasons-for-using-branches)
- [Branches](#branches)
- [How to Create a Branch](#how-to-create-a-branch)
- [Workflow Overview](#workflow-overview)
- [Fork and Pull Model](#fork-and-pull-model)
- [Shared Repository Model](#shared-repository-model)
- [Bash Commands](#bash-commands)
- [Local Development Environment](#local-development-environment)
- [Cloning](#cloning)
- [Changing Directory](#changing-directory)
- [GitHub Repo Versus Local Directory](#github-repo-versus-local-directory)
- [Verifying Branch](#verifying-branch)
- [Creating a New Branch](#creating-a-new-branch)
- [Working on a File Locally](#working-on-a-file-locally)
- [Adding and Committing](#adding-and-committing)
- [Pushing](#pushing)
- [New Branch](#new-branch)
- [Workflow Overview](#workflow-overview)
- [Pull Request Review Process](#pull-request-review-process)
- [Pull Request Command Line](#pull-request-command-line)
- [Pull Request Review](#pull-request-review)
- [Workflow Overview](#workflow-overview)
- [Sandboxing](#sandboxing)
- [Simple, But Effective](#simple-but-effective)
- [Pushing Commits to a Pull Request](#pushing-commits-to-a-pull-request)
- [Triaging](#triaging)
- [Finding Community Projects Versus Via GitHub Search](#finding-community-projects-versus-via-github-search)
- [When You Locate a Project](#when-you-locate-a-project)
- [Documentation](#documentation)
- [Newcomer Perspective is Valuable](#newcomer-perspective-is-valuable)
- [When You Get Stuck](#when-you-get-stuck)
- [Thank You](#thank-you)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script

The script is a general outline and varies somewhat from what was said during the talk.

<table>

<tr><td width="30%">

![Slide 1](https://speakerd.s3.amazonaws.com/presentations/cf52ec3929b04ff58903df5071b56079/slide_0.jpg)

</td><td>

### Get a Jumpstart on Collaboration and Code Review in GitHub 

By Katherine "Kati" Michel

</td></tr>


<table>

<tr><td width="30%">

![Slide 2](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_1.jpg)

</td><td>

### Welcome

* Welcome, everyone. I’m Kati Michel. I'm thrilled to have been asked to share this talk with you.
* I’m really hoping that some of what I share today will be life changing for you the way that it has been for me

</td></tr>


<table>

<tr><td width="30%">

![Slide 3](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_2.jpg)

</td><td>

### About Me 

* Pinax Maintainer/Web Developer (open-source Python/Django library of around 80 projects and apps created by Django core devs)
* DjangoCon US Website Co-Chair
* DEFNA (Django Events Foundation North America) Board Member (we oversee the high level details of DjangoCon US and Django outreach across North America)

</td></tr>


<table>

<tr><td width="30%">

![Slide 4](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_3.jpg)

</td><td>

### Talk Goal

* When I first created this talk 3 years ago, I had learned a lot of what is in it from being the DjangoCon US website maintainer
* I wanted to teach other people, especially women, how to get started collaborating and doing code review as quickly as possible.
* I included a lot of screenshots in this talk, because I want people to see what the process looks like, in a way that I didn’t
* I really felt like I was in the dark while I was learning
* I really packed the talk with a lot of knowledge… a lot of this had been difficult to learn and had taken some courage

</td></tr>


<table>

<tr><td width="30%">

![Slide 5](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_4.jpg)

</td><td>

### Good News

* I have good news
* Now that I’ve had the benefit of several years of using what’s in the talk, I’ve improved the talk
* There are a couple of things that I’ve learned that are really important
* This is not about how much you know… it’s about knowing a few things that enable you to be proficient
* There are people who are successful in using Git and GitHub who literally just use the same handful of commands and basic process over and over again
* I’m not trying to discourage you from knowing a lot or improving
* If you start to get discouraged or overwhelmed… just remember that the goal is to figure out a mental model and commands that you can use permanently

Toward the end of the talk, I’m going to have an exercise you can do to get started using these commands in a practical way that will enable you to do a lot

</td></tr>


<table>

<tr><td width="30%">

![Slide 6](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_5.jpg)

</td><td>

### More Good News

* Git and GitHub are a highly valuable, “gateway” skill... becoming proficient leads to many other opportunities
* Not all Git/GitHub usage is public… it’s also used privately
* Knowing how to use Git and GitHub led to me being hired not long after I created this talk

</td></tr>


<table>

<tr><td width="30%">

![Slide 7](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_6.jpg)

</td><td>

### More Good News- Hacktoberfest

* Hacktoberfest is a month long celebration of open source
* If you make four PRs to active projects on GitHub and are do not miss the cut-off, you get a shirt and swag
* It’s a great time to contribute, because projects will be looking for contributors

</td></tr>


<table>

<tr><td width="30%">

![Slide 8](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_7.jpg)

</td><td>

### Announcing TacoFancy

* I want to tell you how I got started using open-source
* I signed up for GitHub in April 2013. My account sat unused for 7 months. I didn’t know how to get started.
* I happened to be looking at Twitter. 
* I saw a tweet from a man named Dan Sinker. He had made a really delicious taco meal and decided to start a project on GitHub to share taco recipes. 
* So I clicked on the link and went to the project to take a look. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 9](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_8.jpg)

</td><td>

### One Life Changing Question

There was one question in the project info that sincerely changed my life: "Are You New to GitHub But Want to Contribute?" 

</td></tr>


<table>

<tr><td width="30%">

![Slide 10](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_9.jpg)

</td><td>

### My First Pull Request

* At the time, I felt like an outsider. This was the encouragement I needed. 
* I became very determined to contribute and submitted my first pull request there.
* I wanted to build on this experience, so I kept using Git and GitHub. I wasn’t very good at it at first
* A lot of what I did was alone in my own account. But I improved. I learned that the mistakes disappear in the history.

</td></tr>


<table>

<tr><td width="30%">

![Slide 11](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_10.jpg)

</td><td>

### DjangoCon US Website as Example Project

* Eventually, I wanted to start contributing to something
* I realized that a lot of conferences were looking for website contributors
* In 2016, I became a DjangoCon US website contributor
* I wanted to become a maintainer. My git skills were leveling off and I recognized that being a maintainer was a valuable skill and I was curious.
* So I just asked if I could learn how to maintain the DjangoCon US website
* The conference leaders wholeheartedly said yes and offered me the role of Website Chair, which I accepted
* That is where I began to learn how to be a maintainer, including how to review/merge PRs
* That led me to write this talk and it’s why I use the DjangoCon US website as an example project in this talk

</td></tr>


<table>

<tr><td width="30%">

![Slide 12](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_11.jpg)

</td><td>

### Prerequisites for Getting Started

* These are the things that will need to be set up to do what is explained in this talk
* At the end of my talk will be a slide with a link to the slides and other useful resources

* Create a free GitHub account online
* Install Git on your computer and set your email and username
* Find and open your command line (a.k.a. terminal) on your computer
* Be able to navigate via command line (See Bash commands)
* You might also want to have a text editor of your choice installed, to use to edit files (I use VS Code)
You will find documentation for all of these things in the Useful Resources section.

</td></tr>


<table>

<tr><td width="30%">

![Slide 13](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_12.jpg)

</td><td>

### Housekeeping

* Even though I use the word “code” in the title, this talk is more about learning the process… to enable you to do more difficult things
* My screenshots will be in Mac OS: in the GitHub docs, there are tabs that can give info specific by OS
* But, I think the high level process I will show you will be the same

</td></tr>


<table>

<tr><td width="30%">

![Slide 14](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_13.jpg)

</td><td>

### What are Git and GitHub?

* GitHub is a website built on the version control software Git. 
* I don’t know if you’ve ever been working on a file and comically saved a million versions… Git does that for you.
* Originally Git was just used in the command line only
* The people who built GitHub basically took Git and integrated the functionality into a user friendly website 

</td></tr>


<table>

<tr><td width="30%">

![Slide 15](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_14.jpg)

</td><td>

### Social Network

GitHub is a social network. You can:
* Make a user profile
* Follow people
* Follow their activity in your newsfeed
* Find interesting projects

</td></tr>


<table>

<tr><td width="30%">

![Slide 16](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_15.jpg)

</td><td>

### Repositories

But the really important part of GitHub is that users can store and work on code together in repositories

</td></tr>


<table>

<tr><td width="30%">

![Slide 17](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_16.jpg)

</td><td>

### Repositories

(Animation)
For example, if you go to the DjangoCon US organization account you will see a list of repos and at the top is the DjangoCon US website repo. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 18](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_17.jpg)

</td><td>

### Repositories

(Animation)
If you click on the name, it’s a hyperlink that will open up the repo and you will see the folders and files filled with the website code that powers the website and you can look through. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 19](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_18.jpg)

</td><td>

### Local Development Environment Example

* This is why it’s it’s going to look very different if you do something on GitHub the website versus in your local development environment
When we are working on code, we can't do everything in the GitHub website (although there is a new product called Codespaces in beta)
* For example, we might want to make a copy of the DjangoCon US website code in the local development environment of our computer, install the necessary software, and run the code in a local browser so that you can add a feature to it, or test a pull request branch.
* There is where Git is very useful. Git is installed in our local development environment and used in the command line of your computer. You can use Git to make a snapshot of your project at any point in time and revert back if needed.
* Here is a screenshot of my local development environment.
* In the background I have GitHub open in the browser
* In front of that, I have my local folder window and my command line

</td></tr>


<table>

<tr><td width="30%">

![Slide 20](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_19.jpg)

</td><td>

### Local Development Environment Example

(Animation)
* I can use the web address (URL) from the GitHub repo in the command line to create a copy of the repo in my local development environment. Making a copy of a repo locally is called cloning.

</td></tr>


<table>

<tr><td width="30%">

![Slide 21](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_20.jpg)

</td><td>

### Local Development Environment Example

(Animation)
* I can make changes and push the changes back to GitHub. 
* Meanwhile, other users can do the same thing on their computers.
I will elaborate on this process later.

</td></tr>


<table>

<tr><td width="30%">

![Slide 22](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_21.jpg)

</td><td>

### Workflow Overview

* Determine which collaboration approach to use (there are two)
* Learn about branches
* Work on a branch in a local development environment, push the branch to GitHub, and submit a pull request
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Hacktoberfest recommendations… how to get started!

</td></tr>


<table>

<tr><td width="30%">

![Slide 23](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_22.jpg)

</td><td>

### Workflow Overview

* Determine which collaboration approach to use (there are two)

</td></tr>


<table>

<tr><td width="30%">

![Slide 24](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_23.jpg)

</td><td>

### The Two Collaborative Development Models

A Collaborative Development Model is a fancy term for how users contribute to a repo. There are two different models. 
* "Shared Repository" Model
* "Fork and Pull" Model
The two different models typically correspond to the two different account types and which model you uses depends on whether you have write permission to the repo. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 25](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_24.jpg)

</td><td>

### The Two Types of Accounts

* To explain these, I’m going to talk about the two different kinds of accounts
* Organization accounts such as the DjangoCon organization that a group of people have access to
* User accounts that one person has access to, such as my own personal account

</td></tr>


<table>

<tr><td width="30%">

![Slide 26](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_25.jpg)

</td><td>

### Write Permission

* There is a thing called “write permission”
* We are not talking about "write" permission in the context of English.
* When a user has write permission to a repo, it means they can make changes directly inside of the repo.

</td></tr>


<table>

<tr><td width="30%">

![Slide 27](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_26.jpg)

</td><td>

### Examples of What Write Permission Will Allow You to Do

* Edit files
* Push branches directly to the repo (instead of via fork)
* Merge and close pull requests

</td></tr>


<table>

<tr><td width="30%">

![Slide 28](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_27.jpg)

</td><td>

### Why We Need Write Permission

* We need write permission because the code inside of a repo can be really valuable

Example: DjangoCon US website is deployed live from the main branch and has a fairly high volume of traffic. 
* We wouldn't want just anyone to be able to go into the DjangoCon repo and directly make changes. 
* Someone could damage the codebase
* So, the repo owner will give a few, trusted people write permission
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 29](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_28.jpg)

</td><td>

### Write Permission and Collaboration Examples

* The way that we contribute to a repo depends on whether we have write permission to the repo

* Let’s go back to the idea of the “Shared Repository” Model.
* A shared repository is typically found in an organization account, because you have a group of maintainers who all have write access to a repo so that they can maintain it. A user account repo can be a shared repo but it’s not as common. I might be wrong.
* For example, the DjangoCon US website repo is a shared repository. When I became a maintainer, I was given write permission to the repo. Along with the other maintainers, who also have write permission, I can make changes directly within the DjangoCon US website repo.

</td></tr>


<table>

<tr><td width="30%">

![Slide 30](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_29.jpg)

</td><td>

### Write Permission and Collaboration Examples

(Animation)
So what happens if you don’t have write permission, but you want to contribute to a repo?
* In that case, you use the “Fork and Pull” Model. 
* This often happens in a user account
* The person who wants to contribute makes a copy of the repo in their own user account. The copy is called a fork. Because the fork is in their own user account, they have write permission to it. 
* For example, when I first came across the DjangoCon US website repo, I wanted to contribute, but I was not a maintainer, so I didn't have write permission. So I forked the DjangoCon US website repo into user account, made a change to it, then submitted a pull request to the Django US website repo. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 31](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_30.jpg)

</td><td>

### How to Fork a Repo

We've gone to the DjangoCon US website repo. 
* Click the "Fork" button
* Try to edit a file in a repository that you do not have write permission to. GitHub will automatically fork the repo to your user account.

</td></tr>


<table>

<tr><td width="30%">

![Slide 32](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_31.jpg)

</td><td>

### How to Fork a Repo

(Animation)
There will be a message notifying you that it is being forked.

</td></tr>


<table>

<tr><td width="30%">

![Slide 33](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_32.jpg)

</td><td>

### Forked Repo

* The forking message will lead you back to your user account.

</td></tr>


<table>

<tr><td width="30%">

![Slide 34](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_33.jpg)

</td><td>

### Forked Repo

(Animation)
* In the list of repos in your account, you will now see an entry for the fork, which will also tell where it was forked from

</td></tr>


<table>

<tr><td width="30%">

![Slide 35](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_34.jpg)

</td><td>

### Forked Repo

(Animation)
* Click on the hyperlink and it will open the repo
* The repo URL will have my user account name in it (that’s called a namespace)
* The fork is an exact copy of the original repo at the time it was forked. I could make any changes I wanted to the fork, including deleting it, and the original repo will not be affected. 
* In addition to using a fork to propose a change to the original repo, you can also use a fork for the starting point of a new idea of your own (depending on the license). 

</td></tr>


<table>

<tr><td width="30%">

![Slide 36](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_35.jpg)

</td><td>

### Workflow Overview

* Determine which collaboration approach to use (there are two)
* Learn about branches

</td></tr>


<table>

<tr><td width="30%">

![Slide 37](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_36.jpg)

</td><td>

### Collaboration and Code Review Best Practice Workflow Using Branches

* So, you’ve identified how you are going to contribute… through a shared repo or a fork of it
* I want to tell you about branches, which are a best practice
* Branches are very commonly used
* Whatever repo you are working within, you are probably going to want to use a branch to contribute

</td></tr>


<table>

<tr><td width="30%">

![Slide 38](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_37.jpg)

</td><td>

### Working on a File in GitHub

* When I first started using GitHub, I would go into my own GitHub repo, click on a file, click on the pencil icon to open the file, make a change, and save it. 
* This is fine, but imagine if there were multiple people all working on a repo and all of them were going into files and making changes and saving them. It wouldn't be very practical. For instance, how would you give feedback? 
* As the complexity of a project increases, within the repo, we need to make copies of the codebase to work on the code. These copies are called branches.
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 39](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_38.jpg)

</td><td>

### Reasons for Using Branches

* There are multiple benefits to using branches
* To keep your main branch stable
* To work on features outside of the main branch, which may also take time
* So that you can test and review code before merging it into your main branch
 
</td></tr>


<table>

<tr><td width="30%">

![Slide 40](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_39.jpg)

</td><td>

### Branches

* When you create or fork a repo, the default branch is probably called master (or main)
* By the way, GitHub has recently given the option to go into your account settings and tick a box to make the default branch as main, instead of master, due to the historical context of that word
* I highly recommend doing that and I have changed references in this talk from master to main

</td></tr>


<table>

<tr><td width="30%">

![Slide 41](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_40.jpg)

</td><td>

### Branches

(Animation)
Say for instance that you want to make a change in the branch, you can make a new branch (which is a copy of the original branch) and give it a different name. Now there are two branches, in the same repo, the main branch and a feature branch (GitHub will also refer to a feature branch as a topic branch).

</td></tr>


<table>

<tr><td width="30%">

![Slide 42](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_41.jpg)

</td><td>

### Branches

(Animation)
You can create an unlimited number of branches and you can switch in between them to work on them (in the browser and locally).

</td></tr>


<table>

<tr><td width="30%">

![Slide 43](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_42.jpg)

</td><td>

### Branches

(Animation)
When the feature branch author thinks it's done, a pull request will be submitted and the feature branch will become a pull request branch. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 44](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_43.jpg)

</td><td>

### Branches

(Animation)
If the changes are accepted, they will be merged into the main branch. The main branch will be like before, except with the changes from the feature branch.  
* The PR request branch is the same as a regular branch… matters as a maintainer. We can do some of the same things to it, such as push changes to it

</td></tr>


<table>

<tr><td width="30%">

![Slide 45](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_44.jpg)

</td><td>

### How to Create a Branch

Let's go back to the screenshot of editing a file in GitHub. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 46](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_45.jpg)

</td><td>

### How to Create a Branch

(Animation)
There is a radial button you can choose to indicate you want to create a new branch. There is also a place to give the branch a new name. When you click to save the changes, they will not save in the current file. Instead, a new branch will be created. 
* You can also create a branch through the branch button (this will be an exact copy with a new name)
* You can also create and work on branches through the command line in your local development environment, which I will show you later. 
* Anytime I talk about pushing to a repo or submitting a pull request, you should probably be using a branch

</td></tr>


<table>

<tr><td width="30%">

![Slide 47](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_46.jpg)

</td><td>

### Workflow Overview

* Determine which collaboration approach to use (there are two)
* Learn about branches
* Work on a branch in a local development environment, push the branch to GitHub, and submit a pull request

</td></tr>


<table>

<tr><td width="30%">

![Slide 48](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_47.jpg)

</td><td>

### Fork and Pull Model

I've made a couple of diagrams that I hope will give you an idea of what the process is for working locally for each collaborative development model. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 49](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_48.jpg)

</td><td>

### Fork and Pull Model

(Animation)
* Fork the repo

</td></tr>


<table>

<tr><td width="30%">

![Slide 50](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_49.jpg)

</td><td>

### Fork and Pull Model

(Animation)
* Clone the fork (using the fork URL)
Git will track some details about the project, for instance, where we cloned our code from. In relation to the clone, the GitHub repo we cloned from is now a remote repo and Git will assign the name "origin" to it. We can use the name origin in the command line to refer to the repo so we can push and pull changes back and forth between the local development environment and the GitHub repo.

</td></tr>


<table>

<tr><td width="30%">

![Slide 51](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_50.jpg)

</td><td>

### Fork and Pull Model

(Animation)
* Make our changes, push the changes back to the fork (probably in a branch)

</td></tr>


<table>

<tr><td width="30%">

![Slide 52](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_51.jpg)

</td><td>
    
### Fork and Pull Model

(Animation)
* Submit the pull request

</td></tr>


<table>

<tr><td width="30%">

![Slide 53](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_52.jpg)

</td><td>

### Shared Repository Model

Here's what it looks like when we use the "Shared Repository" Model

</td></tr>


<table>

<tr><td width="30%">

![Slide 54](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_53.jpg)

</td><td>

### Shared Repository Model

(Animation)
* The fork is not needed, because we have write permission
* Clone the shared repository (using the shared repo URL). The shared repository will now be the remote "origin"

</td></tr>


<table>

<tr><td width="30%">

![Slide 55](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_54.jpg)

</td><td>

### Shared Repository Model

(Animation)
* Make our changes, probably in a branch, push the changes back to the shared repository
* Submit the pull request

</td></tr>


<table>

<tr><td width="30%">

![Slide 56](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_55.jpg)

</td><td>

### Bash Commands

In GitHub, we navigate using the browser. In the local development environment, we need to use the command line to navigate directories

We can use Bash commands to do that. The commands below are enough to be able to use git. The other commands we are going to use in this talk are git commands.

A couple useful things to know
* Some tasks vary by operating system- check tabs at the top of GitHub articles for special OS instructions; For instance, not all command lines use a $
* <variable> is a placeholder for the real thing

</td></tr>


<table>

<tr><td width="30%">

![Slide 57](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_56.jpg)

</td><td>

### Local Development Environment

What I'm going to show you now is a generic process that you can use for a shared repository or a fork. You will clone the repo you have write permission to.
Let's go back to the screenshot of my local development environment. 
* I am working in my home directory. The name of home directory is at the top of the command line, and in front of the prompt. The reason why this matters is because the repo will be cloned into the directory we are working in, based on my command line.

</td></tr>


<table>

<tr><td width="30%">

![Slide 58](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_57.jpg)

</td><td>

### Cloning

(Animation)
* I am going to type the command $ git clone into the command line and copy and paste the URL from the browser of either the shared repo or fork, then hit enter. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 59](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_58.jpg)

</td><td>

### Cloning

(Animation)
* A folder will appear in my home directory by the same name as the GitHub repo (2017.djangocon.us) and filled with the contents of the repo. 
* This is the equivalent of the repo on the computer now
* I now have a copy of the code online in the GitHub repo and a copy in my local development environment. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 60](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_59.jpg)

</td><td>

### Changing Directory

(Animation)
* I will now change directory into the folder so that I can work there by typing $ cd 2017.djangocon.us, which is a bash command and the folder name.

</td></tr>


<table>

<tr><td width="30%">

![Slide 61](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_60.jpg)

</td><td>

### Changing Directory

(Animation)
* I've clicked on the folder in the folder window so that I can see the contents visually. But I can also see I am working from within the folder in my command line because the name of the folder is at the top of the command line and in front of the prompt. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 62](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_61.jpg)

</td><td>

### GitHub Repo Versus Local Directory

(Animation)
* You can pull up your GitHub repo and your local folder and compare the files. You can see the corresponding files. The format will be slightly different between one set is being rendered in the browser, and another set are raw files. (.gitignore)

</td></tr>


<table>

<tr><td width="30%">

![Slide 63](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_62.jpg)

</td><td>

### Verifying Branch

(Animation)
* If you have more than one branch in the repo that you just cloned, you can switch between branches using your command line
* Use the command $ git branch to verify which branch you are checked out on; initially, you will be checkout out on the default branch (in this case main)

</td></tr>


<table>

<tr><td width="30%">

![Slide 64](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_63.jpg)

</td><td>

### Creating a New Branch

(Animation)
* If you need to make a new branch, you can also do that through the command line and we will later push it to GitHub and it will be just like a branch we create through GitHub website
* Create and checkout (switch) to a feature branch. We are calling this feature branch example-branch. We want to branch off of the branch we intend our changes to be merged into (note how the local files switch to the files of the branch you are checked out on, exactly the same at first, because a copy, but if you make a change in a branch and then switch back and forth between branches, you can see the difference)
* If the branch already exists and you are just switching to it, you leave out the -b

</td></tr>


<table>

<tr><td width="30%">

![Slide 65](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_64.jpg)

</td><td>

### Working on a File Locally

(Animation)
* Open a file in the text editor. Make your change and save it.

</td></tr>


<table>

<tr><td width="30%">

![Slide 66](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_65.jpg)

</td><td>

### Adding and Committing

(Animation)
* In order for the change to become permanent, we need to commit it to Git version control
* Add and commit our change, create a message "Creating branch and updating"
* Be aware that there are other commands that can be used to add files… some people do not like to use the dot (not enough control over what is committed)

</td></tr>


<table>

<tr><td width="30%">

![Slide 67](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_66.jpg)

</td><td>

### Pushing

(Animation)
* Push the new branch named example-branch to GitHub to your origin (the repo you cloned from that you have write permission to)

</td></tr>


<table>

<tr><td width="30%">

![Slide 68](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_67.jpg)

</td><td>

### New Branch

When you go to the repo that is your origin, there will now be a new branch in that repo and a message telling you it's there. The branch will not be affecting anything else. It's just there. If you click on the branch tab you can choose the name of the branch to switch to the new branch. 
* You can also create a branch through the branch tab

</td></tr>


<table>

<tr><td width="30%">

![Slide 69](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_68.jpg)

</td><td>

### New Branch

(Animation)
You can toggle back and forth between the branches by clicking on the branches in the branches tab. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 70](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_69.jpg)

</td><td>

### Submit a Pull Request

Go to the repo you want your pull request to be merged into, in this case, the DjangoCon US website repo. The reason why I say this is because you can accidentally submit a pull request to yourself in your fork. In the DjangoCon US website repo, there will also be a message here telling you about the branch and suggesting that you submit a pull request, even if the branch is in a fork, because GitHub will detect it. Click on the "Compare & pull request" button. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 71](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_70.jpg)

</td><td>

### Submit a Pull Request

(Animation)
* Make sure that the base branch is the branch you want your change to be merged into
* Make sure compare branch is your branch
* Create a pull request title and perhaps a description (some projects also use PR templates)
* If the pull request is via a forked repo, a box will be checked by default giving maintainers the ability to edit the pull request 
* Double check your changes
* Click "Create pull request"

</td></tr>


<table>

<tr><td width="30%">

![Slide 72](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_71.jpg)

</td><td>

### Workflow Overview

* Determine which collaboration approach to use (there are two)
* Learn about branches
* Work on a branch in a local development environment, push the branch to GitHub, and submit a pull request
* Review the two different types of pull requests as a DjangoCon US website repo maintainer

</td></tr>


<table>

<tr><td width="30%">

![Slide 73](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_72.jpg)

</td><td>

### Pull Request Review Process

* Now we are going to switch perspectives and pretend that we are a maintainer
* When a pull request is submitted repo maintainers will receive a notification by browser or email to let them know there is a pull request
* Follow the link to the pull request tab in the browser
* Look over the information about the pull request. You can see the title and description and click on the “Files changed” link to see all of the changes that were made. 

</td></tr>


<table>

<tr><td width="30%">

![Slide 74](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_73.jpg)

</td><td>

### Pull Request Review Process

(Animation)
Underneath that will be:
* A link that says “command line instructions” 
* A merge button that you can click to merge in the browser, when you are ready
There are a few things that can happen
* The simplest scenario is that the change is simple enough (like a typo) that you can just click merge
* You can also ask the person who submitted the pull request to make a change

</td></tr>


<table>

<tr><td width="30%">

![Slide 75](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_74.jpg)

</td><td>

### Pull Request Command Line

There are some situations though where you need to fetch the pull request branch into your local development environment so you can run the code or run a test or work on the code in order to be able to merge it.
When you click on the “command line instructions” link, it will open up a set of instructions for how to review and (possibly) merge the pull request in your local development environment. The instructions will be different depending on whether the pull request was submitted from within the shared repository or from a forked repo. The instructions are different because Git handles shared repos and forks differently locally. This is kind of irrelevant though.

</td></tr>


<table>

<tr><td width="30%">

![Slide 76](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_75.jpg)

</td><td>

### Pull Request Review

There is some overlap in terms of the merge button and the command line instructions
* If you follow the entire instruction set, you will manually merge the pull request branch locally into the branch it is intended to merge with and push it to that branch on GitHub
* I don’t do that. I just follow the instructions to fetch the branch.
* If I verify that it can be merged, I ignore the rest of the instructions and go back to the GitHub PR tab and click the merge button
* The branch might be protected and you can revert the PR
* The part in black is what I do. I do not do the merge/push part.

</td></tr>


<table>

<tr><td width="30%">

![Slide 77](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_76.jpg)

</td><td>

### Workflow Overview

* Determine which collaboration approach to use (there are two)
* Learn about branches
* Work on a branch in a local development environment, push the branch to GitHub, and submit a pull request
* Review the two different types of pull requests as a DjangoCon US website repo maintainer
* Hacktoberfest recommendations… how to get started!

</td></tr>


<table>

<tr><td width="30%">

![Slide 78](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_77.jpg)

</td><td>

### Sandboxing

This is the advice I wish I had had:
* Create a repo in your own GitHub user account (this can public or private)
* Use it to practice the your workflow until you feel confident to use it to contribute to a project
* GitHub has a basic tutorial called Hello World… you can use it to create a repo, a branch, submit a pull request, and merge it
* I have included this link in the Useful Resources and you might be interested in it
* But everything in that tutorial happens in the browser
* You can do make some contributions in the browser only… but there is a limit to what you can do there
* If working in the browser only is what you feel comfortable with, that’s totally fine
* You should do whatever works for you
* The reason why I’m talking about the local dev environment is that it enables you to do more and it’s getting into more of what a dev environment is like
* If it’s something you don’t feel comfortable doing today, it’s maybe something to work toward

</td></tr>


<table>

<tr><td width="30%">

![Slide 79](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_78.jpg)

</td><td>

### Simple, But Effective

* Continuing with this idea of using a sandbox repo to practice
* I would suggest that you use this sandbox repo to work on a branch in the local dev environment similarly to what I demonstrated earlier
* This slide and the next one are literally the process that is the basis for making a contribution from your local dev environment

</td></tr>


<table>

<tr><td width="30%">

![Slide 80](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_79.jpg)

</td><td>

### Simple, But Effective

After this you understand how to do this, you are going to go find a project to contribute to, for it, and use this process to contribute.

</td></tr>


<table>

<tr><td width="30%">

![Slide 81](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_80.jpg)

</td><td>

### Pushing Commits to a Pull Request

* You can also submit a pull request to yourself and use the command line instructions (but if the branch is local, you can’t fetch it)
* You might also want to practice pushing a change to the pull request branch
* The good news is that pull request branches are regular branches
* You can push changes to the pull request branch up to the point that the PR is merged… the changes will be added to the PR
* I’ve included a bit of code in the Useful Resources that can be used to push a change to a forked repo PR branch
* If the contributor has left the box checkmarked giving you permission to edit the pull request 

</td></tr>


<table>

<tr><td width="30%">

![Slide 82](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_81.jpg)

</td><td>

### Triaging

Tips for getting started
In the Useful Resources section there is an excellent checklist for evaluating a project and I recommend that you take a look at it. In general...
I recommend that when you are looking for a project to contribute to:
* Search by tag to find projects that use triaging. Triaging is where issues are sorted by difficulty level
* Maintainers will be creating “hacktoberfest” labels
* Be aware for “help wanted” that these can be their *problem* issues
* As a collaborator or code reviewer, you can cherry-pick issues and pull requests that fit your skill level

</td></tr>


<table>

<tr><td width="30%">

![Slide 83](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_82.jpg)

</td><td>

### Finding Community Projects Versus Via GitHub Search

* Instead of finding projects through GitHub search, considering finding them through your community instead
* One year, my local developer community collected a list of local projects
* A lot of the projects were for non-profits and didn’t have proper docs and other stuff
*  My contributions that year were really nice README.mds with installation instructions.

</td></tr>


<table>

<tr><td width="30%">

![Slide 84](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_83.jpg)

</td><td>

### When You Locate a Project

* It’s a good idea to…
* Use the GitHub Open Source Guide Contributing Checklist
* Look for a CONTRIBUTING.md (might be in the .github repo… will tell you how they want you to contribute)
Let them know if you (in issue):
* Find an issue you want to take
* Think of a feature that you want to add

</td></tr>


<table>

<tr><td width="30%">

![Slide 85](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_84.jpg)

</td><td>

### Documentation

I hope that you will make your project documentation and attitude toward community members welcoming and positive. This is a way to increase the number of contributions and increase diversity. You can go to the Useful Resources Section, follow the links to the DjangoCon US website repo documentation and use them as examples. Documentation is considered extremely useful, but is often missing.
* README.md- gives general project information
* LICENSE- tells you the legal terms under which you can contribute and use the code
* CODE_OF_CONDUCT.md- a set of rules outlining the expectations and responsibilities of contributors 
* CONTRIBUTING.md- gives info about contributing. (look for .github repo)

</td></tr>


<table>

<tr><td width="30%">

![Slide 86](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_85.jpg)

</td><td>

### Newcomer Perspective is Valuable

* Improve things for the next person
* Project veterans may be unable to see the project through the eyes of a beginner
* Create installation docs (often lacking or written for a different OS)

</td></tr>


<table>

<tr><td width="30%">

![Slide 87](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_86.jpg)

</td><td>

### When You Get Stuck

It’s inevitable that you will have moments of frustration and get stuck… here are a few places where you can find help
* Google
* Stack Overflow
* GitHub docs
* Git docs
* Atlassian and GitLab docs

</td></tr>


<table>

<tr><td width="30%">

![Slide 88](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_87.jpg)

</td><td>

### Thank You
Go for it everyone… I remember at the time set up an open source account, thinking to myself that 
Feel free to contact me. If you make progress based on my talk, I'd love to know. Send me a note if you get the chance.

Useful Resources: 
https://git.io/JU2AR

* Twitter handle: @KatiMichel
* GitHub username: KatherineMichel

</td></tr>

</table>

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>


## Useful Resources

### Links

GitHub
* [GitHub](https://github.com)

Getting Set Up
* [Using Git](https://docs.github.com/en/github/using-git)
* [Getting Started Using Git and GitHub](https://docs.github.com/en/github/using-git/getting-started-with-git-and-github)
* [Set Up Git](https://docs.github.com/en/github/getting-started-with-github/set-up-git)
* [Getting Started Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

Git Official 
* [Git Homepage](https://git-scm.com)
* [Git Doc (Docs and Pro Git Book](https://git-scm.com/doc)
* [Git Documentation](https://git-scm.com/documentation)
* [Git Pro Git Book](https://git-scm.com/book/en/v2)

Glossaries and Cheatsheets (FYI, the cheatsheet uses "Desktop" installation)
* [GitHub Glossary](https://help.github.com/articles/github-glossary)
* [GitHub Git Cheatsheet](https://docs.github.com/en/github/getting-started-with-github/git-cheatsheet)
* [Git Cheatsheet](https://training.github.com/downloads/github-git-cheat-sheet.pdf)

GitHub Help and Training
* [GitHub Docs](https://docs.github.com/en/github)
* [GitHub Guides](https://guides.github.com)
* [GitHub Training Guides YouTube](https://www.youtube.com/githubguides)

GitHub Try
* [Try Git](https://try.github.io)
* [GitHub Bootcamp](https://help.github.com/categories/bootcamp) 
* [GitHub Hello World Tutorial](https://guides.github.com/activities/hello-world)

GitHub Learning Resources
* [Git and GitHub Learning Resources](https://docs.github.com/en/github/getting-started-with-github/git-and-github-learning-resources)

GitHub Open Source Guides
* [Open Source Guide](https://opensource.guide)
* [A Checklist Before You Contribute](https://opensource.guide/how-to-contribute/#a-checklist-before-you-contribute)

Collaborative Development Models and Permission Levels
* [About Collaborative Development Models](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-collaborative-development-models)
* [Permission Levels for an Organization](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/permission-levels-for-an-organization)
* [Repository Permission Levels for an Organization](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams/repository-permission-levels-for-an-organization)
* [Permission Levels for a User Account Repository](https://docs.github.com/en/github/setting-up-and-managing-your-github-user-account/permission-levels-for-a-user-account-repository)

Pull Request Branches Created from a Fork
* [Allowing Changes to a Pull Request Branch Created from a Fork](https://help.github.com/articles/allowing-changes-to-a-pull-request-branch-created-from-a-fork)
* [Committing Changes to a Pull Request Branch Created from a Fork](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/committing-changes-to-a-pull-request-branch-created-from-a-fork)

Advanced Collaborative Development Workflow Examples
* [GitHub Flow](https://guides.github.com/introduction/flow/)
* Git Flow
* [A Successful Git Branching Model](http://nvie.com/posts/a-successful-git-branching-model) (more advanced)
* [A Successful Git Branching Model Considered Harmful](https://barro.github.io/2016/02/a-succesful-git-branching-model-considered-harmful)
* [SemVer](http://semver.org) (subtopic)

10x Results
* ["Survey: Getting to 10x — What do the Best Developers Have in Common?"](https://medium.com/javascript-scene/survey-getting-to-10x-what-do-the-best-developers-have-in-common-4c9b4a4915a9)
* [Open Source Guide Insights](http://opensourcesurvey.org/2017/#insights)

Documentation
* [DjangoCon US Website README.md](https://github.com/djangocon/2017.djangocon.us/blob/master/README.md)
* [DjangoCon US Website LICENSE](https://github.com/djangocon/2017.djangocon.us/blob/master/LICENSE)
* [DjangoCon US Website CODE_OF_CONDUCT.md](https://github.com/djangocon/2017.djangocon.us/blob/master/CODE_OF_CONDUCT.md)
* [DjangoCon US Website CONTRIBUTING.md](https://github.com/djangocon/2017.djangocon.us/blob/master/CONTRIBUTING.md)

GitHub Documentation Resources
* [About READMEs](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/about-readmes)
* [Licensing a Repository](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/licensing-a-repository)
* [Adding a License to a Repository](https://docs.github.com/en/github/building-a-strong-community/adding-a-license-to-a-repository)
* [Adding a Code of Conduct to Your Project](https://help.github.com/articles/adding-a-code-of-conduct-to-your-project)
* [GitHub Pages](https://pages.github.com/)
* [Getting Started with GitHub Pages](https://help.github.com/categories/github-pages-basics)
* [Documenting Your Project with Wikis](https://docs.github.com/en/github/building-a-strong-community/documenting-your-project-with-wikis)
* [Editing and Sharing Content with Gists](https://docs.github.com/en/github/writing-on-github/editing-and-sharing-content-with-gists)

Writing and Formatting
* [Getting Started with Writing and Formatting on GitHub](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github)
* [Working with Advanced Formatting](https://docs.github.com/en/github/writing-on-github/working-with-advanced-formatting)

Setting Up and Maintaining Teams
* [Setting Up and Managing Organizaitons and Teams](https://docs.github.com/en/github/setting-up-and-managing-organizations-and-teams)

Recover a Branch
* [Can I Recover Branch After its Deletion in Git?](https://stackoverflow.com/questions/3640764/can-i-recover-branch-after-its-deletion-in-git)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Contact Kati

* Email: kthrnmichel@gmail.com
* GitHub: https://github.com/KatherineMichel
* Twitter: https://twitter.com/KatiMichel

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Copyright

© 2020 to Present Katherine Michel. All Rights Reserved.
