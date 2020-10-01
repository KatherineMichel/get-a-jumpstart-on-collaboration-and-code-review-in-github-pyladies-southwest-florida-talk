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
- [Goal](#goal)
- [Announcing TacoFancy](#announcing-tacofancy)
- [The One Sentence that Motivated Me to Start Using GitHub](#the-one-sentence-that-motivated-me-to-start-using-github)
- [My First Pull Request](#my-first-pull-request)
- [DjangoCon US Website as Example Project](#djangocon-us-website-as-example-project)
- [Prerequisites for Getting Started](#prerequisites-for-getting-started)
- [What are Git and GitHub?](#what-are-git-and-github)
- [Social Network](#social-network)
- [Repositories](#repositories)
- [Local Development Environment Example](#local-development-environment-example)
- [Collaboration and Code Review Best Practice Workflow](#collaboration-and-code-review-best-practice-workflow)
- [Working on a File in GitHub](#working-on-a-file-in-github)
- [Branches](#branches)
- [How to Create a Branch](#how-to-create-a-branch)
- [Overview](#overview)
- [Section 1](#section-1)
- [The Two Collaborative Development Models](#the-two-collaborative-development-models)
- [The Two Types of Accounts](#the-two-types-of-accounts)
- [Write Permission](#write-permission)
- [Examples of What Write Permission Will Allow You to Do](#examples-of-what-write-permission-will-allow-you-to-do)
- [Why We Need Write Permission](#why-we-need-write-permission)
- [Write Permission and Collaboration Examples](#write-permission-and-collaboration-examples)
- [How to Fork a Repo](#how-to-fork-a-repo)
- [Forked Repo](#forked-repo)
- [Section 2](#section-2)
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
- [Submit a Pull Request](#submit-a-pull-request)
- [Section 3](#section-3)
- [Pull Request Review Process](#pull-request-review-process)
- [Pull Request Command Line](#pull-request-command-line)
- [Pull Request Review Options](#pull-request-review-options)
- [Pull Request Branches](#pull-request-branches)
- [Pull Request Review](#pull-request-review)
- [Merge Pull Request Locally and Push to Master Branch](#merge-pull-request-locally-and-push-to-master-branch)
- [Tidy Up](#tidy-up)
- [Advanced Topics](#advanced-topics)
- [Section 4](#section-4)
- [Common Adding and Committing Commands](#common-adding-and-committing-commands)
- [Manual Updates](#manual-updates)
- [Fetching Versus Pulling](#fetching-versus-pulling)
- [Syncing a Forked Repo Clone](#syncing-a-forked-repo-clone)
- [Syncing a Shared Repo Clone](#syncing-a-chared-repo-clone)
- [Adding a Remote Upstream](#adding-a-remote-upstream)
- [Syncing Commands](#syncing-commands)
- [Common Syncing Scenarios](#common-syncing-scenarios)
- [GitHub Flow](#github-flow)
- [Another Workflow](#another-workflow)
- [Learn More About Workflow](#learn-more-about-workflow)
- [Common Branch Commands](#common-branch-commands)
- [Section 5](#section-5)
- [Documentation](#documentation)
- [Code Safety](#code-safety)
- [Additional Safety Considerations](#code-safety-considerations)
- [Productivity Tips](#productivity-tips)
- [Triaging](#triaging)
- [Sandboxing](#sandboxing)
- [Getting Help](#getting-help)
- [Debunking Myths](#debunking-myths)
- [Go For It!](#go-for-it)
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

### Good News

* Git and GitHub are a highly valuable, “gateway” skill... becoming proficient leads to many other opportunities
* Not all Git/GitHub usage is public… it’s also used privately
* Knowing how to use Git and GitHub led to me being hired not long after I created this talk

</td></tr>


<table>

<tr><td width="30%">

![Slide 7](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_6.jpg)

</td><td>

### Hacktoberfest

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

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 19](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_18.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 20](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_19.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 21](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_20.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 22](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_21.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 23](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_22.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 24](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_23.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 25](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_24.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 26](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_25.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 27](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_26.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 28](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_27.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 29](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_28.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 30](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_29.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 31](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_30.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 32](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_31.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 33](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_32.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 34](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_33.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 35](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_34.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 36](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_35.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 37](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_36.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 38](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_37.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 39](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_38.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 40](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_39.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 41](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_40.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 42](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_41.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 43](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_42.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 44](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_43.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 45](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_44.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 46](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_45.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 47](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_46.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 48](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_47.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 49](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_48.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 50](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_49.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 51](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_50.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 52](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_51.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 53](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_52.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 54](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_53.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 55](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_54.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 56](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_55.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 57](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_56.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 58](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_57.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 59](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_58.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 60](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_59.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 61](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_60.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 62](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_61.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 63](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_62.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 64](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_63.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 65](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_64.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 66](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_65.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 67](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_66.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 68](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_67.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 69](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_68.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 70](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_69.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 71](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_70.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 72](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_71.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 73](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_72.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 74](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_73.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 75](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_74.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 76](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_75.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 77](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_76.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 78](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_77.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 79](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_78.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 80](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_79.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 81](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_80.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 82](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_81.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 83](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_82.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 84](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_83.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 85](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_84.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 86](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_85.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 87](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_86.jpg)

</td><td>

### 

</td></tr>


<table>

<tr><td width="30%">

![Slide 88](https://speakerd.s3.amazonaws.com/presentations/de118609b58d4004b7a402c5a34b3b99/slide_87.jpg)

</td><td>

### 

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

© 2020 Katherine Michel. All Rights Reserved.
