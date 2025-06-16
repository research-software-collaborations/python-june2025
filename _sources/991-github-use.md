# Using Git and Github

## Overview of Git and GitHub 
  [Git](https://git-scm.com/) is a distributed version control system that
was originally created by Linus Torvalds, the original creator of the Linux
operating system.

  A [version control system](https://en.wikipedia.org/wiki/Version_control) 
is a tool that allows use to organize and track the evolution of data files
over time. It is in particular widely used and useful for text files, such 
as the source code for software (in various languages such as Python, C++, ...) 
and documents in formats like LaTeX and markdown. Usually the code or
document files that naturally go together are grouped into entities called 
"repositories".

  A version control system is "distributed" if it enables people working in 
different places (and on different systems/computers) to work on independent 
copies of the data/files and then exchange information about the changes 
they have made.

  [GitHub](https://github.com/) is essentially a [cloud hosting service](https://en.wikipedia.org/wiki/GitHub) for git repositories, with some additional 
functionality that becomes important when there are multiple or many 
people developing a piece of softwarew and/or many users of that software.
This includes functionalities for tracking bugs, feature requests and 
continous integration of code changes and testing.

  For the purposes of the exercises in this course, we have a fairly 
simple situation: you have created a Git repository on GitHub and in order
to make changes you are making a clone of that repository either on a 
(transient!) BinderHub instance or on your laptop. Because the BinderHub
instance is transient (it will go away), you periodically want to push any
changes or new code you make to the GitHub (cloud) repository. Even if
you are working on your laptop, pushing to the GitHub repository is useful
to back up your code and to make it visible to others.

## Git and GitHub In Practice 

  Each time you start a new, fresh BinderHub instance (or the very first
time you begin working with Git on your laptop), you will need to:

  * Clone a copy of your GitHub repo on your BinderHub instance or your laptop, you will need to do:

```
git clone https://XXXXX@github.com/pelmer/999-hsf-india-202506-pelmer
```

Here you should substitute "XXXXX" with the github token that we created 
separately, and change the github username and repository name to the one
appropriate for you.

  * You should then change the working directory in JupyterLab (e.g. in
    the filemanager on the left side) to the directory corresponding to
    the Git repo you have just cloned. If you are working in a shell on
    a terminal, you should change your working directory via a command
    like ``cd 999-hsf-india-202506-pelmer`` (or equivalent for your 
    repository name).

  * Execute a couple of commands to tell git some configuration information:

```
git config --global user.email "YOUR-EMAIL@WHEREVER"
git config --global user.name "YOUR NAME"
```

Update the parts in capital letters to your own email and name.

  * Now each time you would like to push any changes you have made locally
    in the BinderHub instance (or your laptop) to the (cloud) GitHub 
    repository, you should:

```
git add FILENAME
git commit -m "SOME SHORT MESSAGE ABOUT WHAT CHANGED"
git push
```

Again change the parts in all capital letters to match what you are doing.
If you have changed more than one file, you can also ``git add`` all of 
those together and then just do a single commit and push:

```
git add FILENAME1
git add FILENAME2
git add FILENAME3
git commit -m "CHANGED SEVERAL THINGS"
git push
```



## Further Information

  For more information and a bit of a deeper dive into things you can do
with git, see websites like:

  * [https://rogerdudler.github.io/git-guide/](https://rogerdudler.github.io/git-guide/)
  * [https://www.atlassian.com/git/tutorials/what-is-version-control](https://www.atlassian.com/git/tutorials/what-is-version-control)
