# Clone bitbucket to gitub

ou can at least manually mirror any Git BitBucket repo from BitBucket to GitHub:

```text
git clone --mirror http://user@bitbucket/user/repo.git
git remote add github http://user@github.com/user/repo.git
git push --mirror github 

// pull branch ทั้งหมด
git remote update
```

\(Create an empty repo on GitHub side first\)

Then, on demand, you can go into your local clone, do a fetch, and then a git `push --mirror github` again to sync new commits.

