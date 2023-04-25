# mint-news

News site for updates to [MINT](https://github.com/mrc-ide/mint) and [mintr](https://github.com/mrc-ide/mintr).

Visit the site at https://mrc-ide.github.io/mint-news

## Install hugo

This needs a recentish version of hugo (at least 0.83), which might not get on with the current reside blog.
The version in apt is probably too old, but snap works (`sudo snap install hugo --channel=extended`)

## Download source

```
git clone --recursive git@github.com:mrc-ide/mint-news
```

## Create a new post

```
hugo new posts/<title>
```

This will create a .md file in `content/posts` which you should edit.

You should edit the following options as required:

```
---
title: "Add a title here"
date: 2023-04-24T13:51:48+01:00
tags: ["Feature"]
version: ["MINT v2.0.1"]
---
```

## Writing posts

Please include a tag in your post header using `tags: ["Feature"]`. Please use one of the following tags:
* Feature - a new feature that users have asked for or will notice
* Update - a smaller update to something in the UI, or a less user facing update change, or a change to logic
* Data - an update to the input data

Include a version with the `version` field (e.g., `version: ["MINT v2.0.1"]` or `version: ["data v20230208""]`).

## Run locally

```
hugo serve
```

Visit http://localhost:1313/mint-news/ to see changes, editing the file will reflect immediately

## Docs

* [Theme docs](https://github.com/adityatelange/hugo-PaperMod)
* [Hugo docs](https://gohugo.io/documentation/)
