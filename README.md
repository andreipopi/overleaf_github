[Link()] to the Gist version of this guideline.
# Write in Overleaf, push to GitHub, and viceversa.

These guideline are a rework and (imo) improvement of information available on the Overleaf wepage (), and from @jnaecker (). It is put together in a way that tightly follows my intuition, and hopefully the one of others, and that answers "silly" doubts one might have.

This is an image of how the flow flows.


The idea is that you work on your paper in Overleaf (unbothered), and stay in sync with a GitHub repo, in which other scientists are doing stuff. To do that, you need to setup the connections in the image, and to use the usual (add, commit, push, pull) commands to keep the "flow" up to date.

Enjoy.


## Starting point

- premium Overleaf
- git installed locally
- an **empty GitHub repo**
- a **project in Overleaf** (in my example i just had a main.tex and a library.bib)


## Setup

You will now need to setup the two remote sources (overleaf and GitHub), so that you can push and pull to/from them.
```git remote overleaf https://git.overleaf.com/65113somenumber```

## Unlicense

This guide is available under The Unlicense. In other words you can do whatever you are pleased with it.




## Regular Workflow
