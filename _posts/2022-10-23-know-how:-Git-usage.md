---
published: true
---

## To creat a repository of an exsisting project in github from your local server:

1. [Create a new repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository) in Github website. **To avoid errors, do not initialize the new repository with README, license, or gitignore files.** (This is important as I did mistakes at the beginning after clicking add README)

2. Use the init command to initialize the local directory as a Git repository. For Git 2.27.1 or an earlier version, set the name of the default branch using && git symbolic-ref HEAD refs/heads/main:
> $ git init && git symbolic-ref HEAD refs/heads/main

3. Add the files in your new local repository. This stages them for the first commit.
> $ git add .

4. Commit the files that you've staged in your local repository.
> $ git commit -m "First commit"

5. At the top of your repository on GitHub.com's Quick Setup page, click  to copy the remote repository URL.

6. In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
> $ git remote add origin _REMOTEURL_ <br/> 
  $ git remote -v  <br/>
  #Verifies the new remote URL  

7. Push the changes in your local repository to GitHub.com.
> $ git push origin main


References:
- [https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github](https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github)


## To merge changes from the remote repo to local, such as after readme file was added in the remote repo:

1. Pulling changes from a remote repository
> $ git pull origin main

## To add the README file locally:

1. First creat the README.md:
> $ touch README.md

2. Then add, commit and push the changes:
> $ git add . <br/> 
  $ git commit -m "added readme"  <br/> 
  $ git push origin main


## To sync with the local, push changes from the local to remote:

1. Add the updated files in your local repository, which tells Git that you want to include all of your changes in the next commit.
> $ git add .

2. Git commit takes a snapshot of those changes.
> $ git commit -m "description of changes"

3. To push the current branch and set the remote as upstream.
> $ git push --set-upstream origin main

## Clone from a remote repository:

> $ git clone _REMOTEURL_


## Push git cloned repository to your own on GitHub:

1. First you need to remove the remote repository associated using git remote rm origin
> $ git remote rm origin

2. Then creat your own repository and do the above procedures.


References:
- [https://docs.github.com/en/get-started/quickstart/contributing-to-projects](https://docs.github.com/en/get-started/quickstart/contributing-to-projects)
