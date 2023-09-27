# Write in Overleaf, push to GitHub, and viceversa.

The idea is that you work on your paper in Overleaf, and stay in sync with a GitHub repo, to which other scientists are contributing. To do that, you need to set up the remote repos (Overleaf and GitHub), and to use the usual (add, commit, push, pull) commands to keep the "flow" up to date.

## Starting point

- premium Overleaf
- Git installed locally
- an **empty GitHub repo**
- a **project in Overleaf** (in my example i just had a main.tex and a library.bib)


## Setup

First, you need to clone the Overleaf project on your local machine, by copying and executing (in your Terminal) the command from the upper right corner (Overleaf): Menu/Git/

- ```git clone https://git.overleaf.com/65113somenumber```

Then, navigate in the newly cloned repo through your Terminal and set up the two remote sources (Overleaf and GitHub), so that you can push and pull to/from them.

- add remote source for Overleaf
  
```git remote overleaf https://git.overleaf.com/65113somenumber```

- add remote source for your empty GitHub repo

```git remote github https://github.com/username/yourrepo.git```

Then locally pull the existing project from Overleaf, and push it to GitHub to have your project synched everywhere.

- ```git pull overleaf master```

At this point you probably have to ```git add``` changed files and ```git commit``` them. Then you are ready to push the changes to GitHub.

- ```git push github master```

Authentication might be required, and you might need to generate a personal access token for the requested password.

## Workflow

- Work on your paper in Overleaf
- ```git pull overleaf master``` to locally pull changes from Overleaf
- ```git push github master``` to push changes to GitHub
- ```git pull github master``` to get changes from GitHub
- ```git push overleaf master``` to push available changes to Overleaf
  
