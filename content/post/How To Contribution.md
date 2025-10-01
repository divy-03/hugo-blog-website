---
title: How to Contribute
description: First time solving 4 questions in div 4

date: 2025-09-14T20:12:52+08:00
lastmod: 2025-09-14T20:12:52+08:00
tags:
  - blog
  - codeforces
  - cpp
  - contest
categories:
  - dsa
---


# How to Contribute

### If you do not have permission for the repo

- Fork the repo you want to contribute to create your own copy.
> Keep your forked repo up to date and synced

- Clone this forked repo to local system
```shell
git clone <repo_url>
cd <repo_name>
```

- Create a branch for feature or fix
```shell
git checkout -b <branch-name>
```

- Then make changes into this branch only and save locally.
> Use your favourite editor to edit, run and test the code.

- Commit & Push changes
```shell
git add -A
git commit -a -m "fix: message"
git push origin <branch-name>
```

- Create a Pull-Request (PR)
> Go to GitHub and click compare & pull request, give a title and submit.

- Wait for Review by Repo Owner or ask them to merge.

### If you have permission to push

- Clone the repo directly
```shell
git clone <repo_url>
cd <repo_name>
```

- Create a branch for feature or fix
```shell
git checkout -b <branch-name>
```

- Then make changes into this branch only and save locally.

- Commit & Push changes
```shell
git add -A
git commit -a -m "fix: message"
git push origin <branch-name>
```

- Open a Pull request
> Even if you have direct push access, opening a PR is recommended. It helps track changes and makes collaboration easier.

- Merge Pull request
> Since you have permissions, you'll see a Merge Pull Request button.

- Choose how to merge
  - Merge commit -> Keeps full history
  - Squash and merge -> Combines all commits into one (cleaner)
  - Rebase and merge -> Replays commits on top of main branch

### Tips for Good Contributions
- Write clear commit message (`feat:`, `fix:`, `docs:`, etc.).
- Keep your branches small and focused on one change.
- Sync regularly with the main repo (`git pull upstream main`).
- Be respectful and responsive in PR discussions.
