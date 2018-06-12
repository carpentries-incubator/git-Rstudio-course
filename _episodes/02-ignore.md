---
title: "Ignore files from version control"
teaching: 5
exercises: 5
questions:
- "How to exclude files and folders from version control"
objectives:
- "Exclude `Rproj` files, draft folders and sensitive information from version control"
keypoints:
- "Adding file names or folder names to `.gitignore` excludes them from version control"
---

## `.gitignore`

When starting a new project in RStudio, it will always add a file `.gitignore` if it does not already exists (you can actually also create one in the online setup) and adds some initial files to ignore. A `.gitignore` file enlists all those files that should not be taken into account by Git (not part of the snapshot). An example is the `myprojectname.Rproj` file (e.g. `DCEcology`), as this is a user/computer specific file.

Hence, we can ignore the `myprojectname.Rproj` file by adding the file to the `.gitignore` text-file. We can do this inside Rstudio.

> ## Ignore a file
> 
> 1. Go to `git` pane (the tab that says Git), 
> 2. Right click on `....Proj` and select `Ignore...`
> 3. Check if the content of `.gitignore` is correctly updated and click `Save`.
> 
> > ## Solution
> >
> > ![Update .gitignore]({{ page.root }}/fig/gitignore-rstudio1.png)
> > 
> > ![Update .gitignore]({{ page.root }}/fig/gitignore-rstudio2.png)
> >
> {: .solution}
{: .challenge}

Some other examples of files you probably want to ignore:
- Sensitive information (passwords,...)!
- Binary files. Git works very will with **text** files (any type of text), but not with binary files such as `.Rdata`.
- Files > 50MB. Git is specifically made for **code** (e.g. R) and does not intend to track all changes in large data files (e;g. csv)
- A _temp/_ folder inside your project with 'disposable' content, e.g. `draft`, `test` or `temp`. Sometimes such a subfolder is convenient, but should not contain anything crucial for your project.
- In any programming language, some files are _derivatives_

> ## Ignore all files inside a folder
>
> 1. Create a folder `plots/` and add an image to the folder.
> 2. Right click on `plots/` and select `Ignore...`
> 3. Check if the content of `.gitignore` is correctly updated and click `Save`.
>
> {: .challenge}

> ## Use wildcards to ignore multiple files
> 
> Note that you can use wild cards e.g. `*.Rproj` to exclude a group of files from the version control.
{: .callout}

 




