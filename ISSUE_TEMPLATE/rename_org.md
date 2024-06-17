---
name: Update repo to new organisation name
about: Use this template for tracking steps required to update repo to new org name.
title: "[ORG NAME CHANGE]: Update repo to hubverse-org organisation name"
labels: orgname-change
assignees: annakrystalli
projects: "hubverse Development overview"
milestone: "org-rename"
---

- [ ] Create new branch called `to-hubverse` from latest dev branch (most likely related to the v3 schema PRs). (Make sure to pull first). If none exist, branch off from `main`.
- [ ] Find and replace `Infectious-Disease-Modeling-Hubs` with `hubverse-org` throughout repo.
- [ ] Replace origin remote to point to the new organisation
    ```bash
    git remote set-url origin https://github.com/hubverse-org/<REPO_NAME>.git
    # Check remotes
    git remote -v
    ```
    ```r
    url <- paste0('https://github.com/hubverse-org/', basename(getwd()), '.git')
    usethis::use_git_remote(name = "origin", url, overwrite = TRUE)
    # Check remotes
    usethis::git_remotes()
    ```
- [ ] Push and open PR to original branch.
