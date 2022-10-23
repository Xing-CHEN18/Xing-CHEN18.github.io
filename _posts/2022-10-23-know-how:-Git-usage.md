---
published: false
---

To creat a repository of an exsisting project in github from your local server:

1. [Create a new repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository) in Github website. **To avoid errors, do not initialize the new repository with README, license, or gitignore files.** (This is important as I did mistakes at the beginning after clicking add README)

2. Use the init command to initialize the local directory as a Git repository. For Git 2.27.1 or an earlier version, set the name of the default branch using && git symbolic-ref HEAD refs/heads/main:

$ git init && git symbolic-ref HEAD refs/heads/main
