# Git for dummies

During one of the Weekly Nerd sessions, Titus Wormer gave a very interesting presentation about Git and its history. When it started I thought I knew a lot about Git, but it surprised me how much I didn't know as a starting developer. For all of you that want to learn more about Git, this is all you need to know to start using it like a pro!

## What is it Git, and who invented it?

Git is a version control system (VCS) that allows you to have different versions of your development project. It keeps track of all the changes you make, so you can easily collaborate in a clear and understandable way. Git is not the only VCS developers can use to maintain their projects. There are others like Fossil, Mercurial and many more (Kenlon, 2016). But Git is the one that most developers use (Atlassian).

Git is an open source project that was developed by Linus Torvalds in the year 2005. Torvalds created the version control system while he was building the Linux Kernel. Originally Git was written in _C, but now it has been build using Java, Ruby and Python as well (Vogel, 2016).

## Deeper dive into Version Control System

When you start a big project as developer you will create a lot of files that you need for the application to work. A VCS like Git makes it possible to track the history of all changes you’ve made during the project. The nice thing is, that it enables collaborations on projects. So, let’s say you want to setup a web application where you want to work on with multiple people. After uploading (committing) your setup, others can collaborate on that. You posted the first version, every change that gets committed after that is a new version. For each version, you can track all changes that are made.

## How does it work?

After downloading the Command-Line-Interface (CLI) you can start using GIT. It begins with creating a repository. This is the place where all your working history is stored. Mostly it contains multiple files and folders within the project you are working on.

Let’s say we’re going to build a simple CMS. We’ll start making a register and login system. Within the repository we now create a branch to start working in. This branch contains the same files as the main repository (called master mostly). The difference is, when you start coding, commit and push the work you’ve done to the new branch, it’s not pushed to the master automatically. In that way you can test your branch until it works perfectly. After that, just merge your branch into the master. So, all the code you’ve written is now part of the main repository.

The fact that you can make branches makes it easy to collaborate. Everyone that works on the same project can now make its own branch. In that way, you’ll never overwrite each other’s code. Well, never is a big word...

## Merge conflicts

A merge conflict is the nightmare of each developer. Let’s say you’ve worked on the ‘Login Screen’ feature branch. After building the new functionalities you commit the work you’ve done and push it to the master branch. Bam! Merge conflict. That means that one of the collaborators worked on the same file. Now Git doesn’t exactly know what lines to keep and which should be ignored. That is called a merge conflict. Now you have to sit together with your colleague to find out what code should stay, and what can be deleted. That could take you some hours!

## Why should I use Git when there is GitHub?

When you are using GitHub, your using Git. But when using Git only, GitHub isn’t used at all. As you can read in this article, Git is the Version Control System with all the functionalities I’ve described. GitHub isn’t Git. It’s just a hosting service for all the repositories you make. It makes it possible for anyone to visit your repository and to see all the commits and branches made using Git trough an interface.

## And there is much more to learn

So, you’ve read the most basic info you can get about Git (and GitHub). There is still a lot to learn. How to make the perfect commit? How to work with issues? And a lot more. I can’t discuss all of that in this article. But just Google it, and you’ll find out there is a lot more you need to know to get the most out of Git!

# Sources

- Atlassian. (n.d.). What is Git . Retrieved 06 25, 2017, from Atlassian: https://www.atlassian.com/git/tutorials/what-is-git
- Kenlon, S. (2016, 07 07). What is Git? Retrieved 06 25, 2017, from Opensource.com: https://opensource.com/resources/what-is-git
- Vogel, L. (2016). Git - Tutorial. Retrieved 06 25, 2017, from Vogella: http://www.vogella.com/tutorials/Git/article.html
