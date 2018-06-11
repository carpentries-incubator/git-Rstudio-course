---
title: "Interact with GitHub"
teaching: 5
exercises: 10
questions:
- "How to sync your files with GitHub"
- "How to get remote changes on your local machine?"
objectives:
- "`Push` updates to GitHub"
- "`Pull` updates from GitHub"
keypoints:
- "`Push` our code to GitHub and `pull` your code from GitHub"
---

## `Push` changes to GitHub

In the previous episode, we explored the difference in between the local commit history and the commit history on the GitHub remote. 

Rstudio gives you a warning about the status of your local commits versus those stored on GitHub.  

![Push]({{ page.root }}/fig/push-rstudio1.png)

> ## Rstudio note on `ahead of`
> 
> If the Git pane displays *your branch is ahead of ‘origin/master’ by X commits*, this is actually providing you a warning message saying there is no backup of these commits!
{: .challenge}

In order to store these changes on GitHub as well, we have to push our changes to GitHub.

> ## Push to GitHub
> 
> 1. Click push in the git pane
> 2. Go to your repository on GitHub to verify the commits and file contents
{: .challenge}

## Store credentials

It is a tedious task to retype the password each time you want to push anything to GitHub. Luckily, you can store your credentials when using https.

> ## Configure password
> 
> 1. Click on the `more` button in the `git` pane and select `Shell`
> 2. Type `git config --global credential.helper store`
> 3. Type `exit` to quit the shell
{: .challenge}

## `Pull` changes from GitHub

When working from different computers or when you adapted some text online in GitHub, it is important to integrate these adaptations on your local computer. To do so, you can `pull` changes from Github.

> ## Pull changes from GitHub
> 
> 1. Update the `README.md` file online and commit the change
> 2. `pull` the changes to your local machine
> 3. Open the `README.md` file in Rstudio and check if the file has changed.
{: .challenge}