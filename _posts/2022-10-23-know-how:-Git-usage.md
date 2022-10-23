---
published: true
---

To creat a repository of an exsisting project in github from your local server:

1. [Create a new repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository) in Github website. **To avoid errors, do not initialize the new repository with README, license, or gitignore files.** (This is important as I did mistakes at the beginning after clicking add README)

2. Use the init command to initialize the local directory as a Git repository. For Git 2.27.1 or an earlier version, set the name of the default branch using && git symbolic-ref HEAD refs/heads/main:
> $ git init && git symbolic-ref HEAD refs/heads/main

3. Add the files in your new local repository. This stages them for the first commit.
> $ git add .

4. Commit the files that you've staged in your local repository.
> $ git commit -m "First commit"

5. At the top of your repository on GitHub.com's Quick Setup page, click  to copy the remote repository URL.

6. In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
> $ git remote add origin <REMOTE_URL>
> $ git remote -v
> #Verifies the new remote URL

7. Push the changes in your local repository to GitHub.com.
> $ git push origin main



