---
title: "Creating a repository"
teaching: 5
exercises: 10
questions:
- "How to start a project with version control?"
objectives:
- "Create a repository on GitHub"
- "Understand the options about README, license and .gitignore"
keypoints:
- "Initiate a new project in GitHub"
- "Start the project in Rstudio from Git"
---

## Create a repository

When working on a project, one typically uses a project folder to contain the project files, scripts and data. In GitHub, such a project folder is called a repository. Hence, a new project starts with a new repository. First of all, you need to sign in to [GitHub.com](https://github.com/login):

![GitHub login]({{ page.root }}/fig/github-login.png)

a new repository or project can be started by either:

- Click `Start a project`
- Click on the `+` sign in the top right corner
- Click `New repository`

![Create a repo on Github]({{ page.root }}/fig/github-new-repo.png)

When creating a repository, some elements need to be defined:

![Create a repo]({{ page.root }}/fig/github-create-a-repo.png)

1. **Repository name**: Choose something meaningful, without spaces
2. **Description**: Short one-line sentence describing what your project is all about
3. **Public/private**: As long as you keep your repository public, GitHub acts as a free service. Remark that some institutes do support an enterprise GitHub or private repos
4. **README.md**: A Readme is a crucial element of a repository, as it provides the introduction information for other users to get started
5. **.gitignore**: This file describes which files that should not be tracked by Git. For the moment, you have not to select this and keep it on None as we will use Rstudio to provide the `.gitignore` file in [episode 2]({{ page.root }}{% link _episodes/02-ignore.md %}).
6. **LICENSE**: for scientific work, a BSD or MIT license are probably most appropriate. Check the [choose a license website](https://choosealicense.com/) for more information on open source licenses. 

> ## Create a repository
> 
> 1. Go to [GitHub](https://github.com) and login
> 2. Follow [this tutorial](https://help.github.com/articles/create-a-repo/) to create a repo and [create your first (online) commit](https://help.github.com/articles/create-a-repo/#commit-your-first-change) to your repository
{: .challenge}

## Clone a repo to work locally

We have initiated a repository online. Hence, we can start working on the code locally by downloading the repository to our computer. Rstudio provides a convenient way to start a new project as a Git repository.

To get the https link, you need to click the green button and make sure to copy paste the link with as title `Clone with HTTPS`:

![Copy the https link of a repo]({{ page.root }}/fig/copy-repo-link.png)

> ## Start new R project from repository
> 
> 1. On your GitHub repository page, copy the repository **HTTPS** url (*check  the green button on your repo page*)
> 2. In Rstudio, `File > New Project...`, select `Version Control`, choose `Git`
> 3. Provide the repository HTTPS link you just copied (the project name will be filled in as well)
> 4. Browse to the desired directory where you will manage your project/code
{: .challenge}

An example of the project setup using an existing Git repository:

![Clone a repo in RStudio]({{ page.root }}/fig/create-project-rstudio.png)

> ## Check folder content on local machine
> 
> In your File explorer, search for your project folder and check the content. Does this corresponds to what is shown online on your repository website?
{: .challenge}






