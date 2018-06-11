---
title: "Ignore files from history"
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

## `.gitignore`

When starting a new project in RStudio, it will always add a file `.gitignore` if it does not already exists (you can actually also create one in the online setup). A `gitignore` file defines all those files that should not be taken into account by Git. An example is the `myprojectname.Rproj` file, as this is a user/computer specific file.

Some other options of files you probably want to ignore:
- Sensitive information (passwords,...)!
- Binary files. Git works very will with **text** files (any type of text), but not with binary files such as `.Rdata`.
- Files > 50MB. Git is specifically made for **code** (e.g. R) and does not intend to track all changes in large data files (e;g. csv)
- A _temp/_ folder inside your project with 'disposable' content, e.g. `draft`, `test` or `temp`. Sometimes such a subfolder is convenient, but should not contain anything crucial for your project.
- In any programming language, some files are _derivatives_

Hence, we can ignore the `myprojectname.Rproj` file by adding the file to the `.gitignore` text-file. We can do this inside Rstudio.

> ## Ignore a file
> 
> 1. Go to `git` pane (the tab that says Git), 
> 2. right click on `....Proj` and select `Ignore...`
> 3. Check if the content of `.gitignore` is correctly updated and click `Save`.
{: .challenge}

Check the content of the `.gitignore` file. If satisfied, click `Save`:

![Update .gitignore]({{ page.root }}/fig/gitignore-rstudio2.png)

> ## Use wildcards to ignore multiple files
> 
> Note that you can use wild cards e.g. `*.Rproj` to exclude a group of files from the version control.
{: .callout}

 




