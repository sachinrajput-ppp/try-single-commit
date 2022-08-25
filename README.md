# try-single-commit

## Using `reset`

```sh
# --------------- Flow - 1
# creating new branch from main
git checkout -b feature1
# do some changes - I
git add .
git commit -m 'changes 1'
# do some changes - II
git add .
git commit -m 'changes 2'
# do some changes - III
git add .
git commit -m 'changes 3'

git reset main
git add .
git commit -m 'all changes(I, II, III)'
git push origin main

# ------ Flow - 2 - combining the commit after pushed to remote
git checkout feature1
# do some changes - IV
git add .
git commit -m 'change 4'
# do some changes - V
git add .
git commit -m 'change 5'

git reset main
git add .
git commit -m 'all the changes(I-V)'
git push -f origin main
```

## Using `rebase`

```sh
```