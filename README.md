[Link()] to the Gist version of this guideline.
# Write in Overleaf, push to GitHub, and viceversa.

The idea is that you work on your paper in Overleaf (unbothered), and stay in sync with a GitHub repo, in which other scientists are doing stuff. To do that, you need to setup the connections in the image, and to use the usual (add, commit, push, pull) commands to keep the "flow" up to date.

## Starting point

- premium Overleaf
- git installed locally
- an **empty GitHub repo**
- a **project in Overleaf** (in my example i just had a main.tex and a library.bib)


## Setup

You need to setup the two remote sources (overleaf and GitHub), so that you can push and pull to/from them.

- add remote source for overleaf
  
```git remote overleaf https://git.overleaf.com/65113somenumber```

- add remote source for your empty GitHub repo

```git remote github https://github.com/username/yourrepo.git```


## Workflow

- Work on your paper in Overleaf
- ```git pull overleaf master``` locally
- ```git push github master``` to push to GitHub
- ```git pull github master``` to get changes from GitHub
- ```git push overleaf master``` to push available changes to Overleaf
  

## Unlicense

This guide is available under The Unlicense. In other words you can do whatever you are pleased with it.




## Regular Workflow
