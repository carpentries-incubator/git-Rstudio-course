---
title: Setup
---


In order to start using version control in Rstudio, we have to do some configuration the first time. You only leed to do this configuration once.

## Installations

1. [Download](https://git-scm.com/downloads) and install Git
1. Install [RStudio](https://inbo.github.io/tutorials/installation-RStudio-admin.html)

## Link Git and Rstudio

First of all, tell RStudio where to find the Git installation. 

1. Go to `Tools > Global Options`
1. Click on `Git/SVN`.
1. Check *Enable version control interface for RStudio projects*
1. Set the path to the Git executable that you installed*
1. Check *use Git bash as shell for Git projects*

If you do not know where Git is installed, open your command line (`cmd` in Start for Windows user). When the cmd is open, type `where git` and hit enter. The path should be something like: `C:/Program Files (x86)/Git/bin/git.exe`. Still in trouble? Check [this out](http://happygitwithr.com/rstudio-see-git.html#tell-rstudio-where-to-find-git).

![RStudio setup for git]({{ page.root }}/fig/RStudio-setup-git.png)

## Github configuration

Next, we have to tell Github who we actually are, in order to make the connection to the online account. To do so, Git requires the configuration of your Github (!) username and GitHub email:

1. Go to `Tools > Shell` to open the Git Shell
1. In the shell, type the following command and enter:
```
git config --global user.name "mygithubusername"
```
1. Still in the shell, type the following command and enter:
```
git config --global user.email "my.name@inbo.be"
```

![RStudio setup git shell]({{ page.root }}/fig/Rstudio-GitShell.png)

> ## Github configuration check
>
> Use your **GitHub username**! You can check if you're set up correctly by typing  in the same shell:
>
> ~~~
> git config --global --list
> ~~~
> {: .source}
> 
> When successful, the configuration is done. Congratulations!
{: .callout}



