---
name: Upgrade Docs to hubStyle
about: Use this template for upgrading your hubverse package docs to use the hubStyle pkg
title: "Upgrade Docs to hubStyle"
labels: docs, hubstyle
assignees: annakrystalli
---

## Update package config

- [ ] Create `enhancement/hubstyle` branch
- [ ] Run `hubDevs::use_hubdev_pkgdown(add_logo = TRUE)` to update pkgdown
- [ ] Add logo to your README
- [ ] Append standard footer to README. Render
- [ ] Run `hubDevs::use_hubdev_community()` to update community docs
- [ ] Run `hubDevs:::hubdev_ignore()` to ignore std files
- [ ] Check authors
- [ ] Add `hubverse` & `r-package` topics to repos

## Set up Netlify PR Previews

- [ ] Log into Hubverse Netlify account and drag in pkg docs direcory to creat new site.
- [ ] Edit site name with `[pkg_name]-pr-previews` and copy `NETLIFY_SITE_ID`
- [ ] _Create a `NETLIFY_AUTH_TOKEN` if required._
- [ ] Add `NETLIFY_AUTH_TOKEN` & `NETLIFY_SITE_ID` to repository secrets


### Push to Github, open a PR and check Preview 🎉
