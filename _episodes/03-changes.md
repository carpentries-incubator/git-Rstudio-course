---
title: "Commit changes"
teaching: 0
exercises: 0
questions:
- "Key question"
objectives:
- "Create a repository on GitHub"
- "Understand the options about README, license and .gitignore"
keypoints:
- "First key point."
---

## Add file and commit changes

### Commit changes to `gitignore`

In Git, changes are tracked by taking snapshots of the project folder, triggered by the user. A snapshot is taken by a `commit`, which is combined with a user defined `commit message`. It logs the user and date/time and defines the changes with the previous commit (added and removed lines/files).

In the previous episode, a  `.gitignore` file was created. The status of the `.gitignore` file before the file is added to the Git history is clarified with the yellow question mark saying that the file is yet unknown to Git:

![Local commit]({{ page.root }}/fig/commit-rstudio1.png)

By checking the box and clicking commit, we add the file and can commit this addition with a commit message:

![Local commit]({{ page.root }}/fig/commit-rstudio2.png)

We get a small technical overview of the alterations we provided with this commit: 

![Local commit]({{ page.root }}/fig/commit-rstudio3.png)

> ## Add the `gitignore` file to the history
> 
> 1. Go to `git` pane
> 1. Check the box next to `.gitignore`
> 1. Click `Commit`
> 1. Add a `commit message` and click commit
> 1. Click `Close` to remove the commit summary
{: .challenge}

### Provide project info in README

It is good practice to commit often, so you will do this a lot. Each commit should only contain changes related to a single problem/element/… Each commit is a snapshot of your project and the messages describe the new ste taken in your project.

As documentation is crucial, providing some more information in the README.md file will help others (and yourself in a couple of months/years) to understand the aim of the project. Just as we adapted the  README.md file online earlier, we can do the same locally.

> ## Update the README of the project
> 
> 1. Update the README.md inside Rstudio
> 2. Commit your changes
{: .challenge}

### Add new files

During a project, new files will be added to the project folder, which need to be version controlled as well. New directories and files can be added and committed, just like any other adaptation.

Remark that we aim to have a clean directory structure in our projects with the data, scripts and output figures separated, for example:

```
- scripts
- data
- images
```

By clicking the box next to a file, the file is staged (i.e. ready to be committed). Staging a new directory will stage all files in the directory. However, you can not stage empty directories!

> ## Add data file to the project
> 
> 1. Add the  surveys.csv file in a /data subdirectory
> 2. Link to this file in the README.md (use relative paths), mentioning the purpose of the file
> 3. Commit both changes (new data file and the README.md adaptation) in a single commit message
> 4. Add and commit an R script as well, but put this into the `scripts` directory.
{: .challenge}

## Create logical commits

As mentioned earlier, you should commit often and make sure each commit links to a specific change/problem. Sometimes, this means that you have to split the additions in a single file into two individual commits. Rstudio provides the interface to include specific lines of code into a commit message.

![Logical commits]({{ page.root }}/fig/logical-commit-rstudio.png)

To summarize, the following actions can be executed:

- `stage xyz`: add the xyz from the commit
- `unstage xyz`: remove the xyz from the commit
- `discard xyz`: revert the changes in the xyz (be careful, can't be undone!)

and `xyz` can be

- a single `line`
- a `selection` of lines
- a `chunk`
    - RStudio will automatically split the changes in chunks
    - chunks are defined by 10 unchanged lines between changes

> ## `commit`  guidelines
> 
> 1. Limit the subject message to 50 characters 
> 2. Capitalize the subject message line 
> 3. Do not end the subject message with a period 
> 4. Use the imperative mood in the subject line
> 5. Use the body to explain what and why vs. how
{: .callout}

> ## Make logical commits
> 
> 1. Make 2 unrelated changes to your R script
> 2. Create one `commit` for each change:
>     1. Select the changes you want to commit and click `stage selection`
>     2. Add a `commit message` and click `Commit`
{: .challenge}















