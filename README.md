# naomi-news

This is the source for our naomi changelog, it will be deployed to https://reside-ic.github.io/naomi-news

## Install hugo

This needs a recentish version of hugo (at least 0.83), which might not get on with the current reside blog. The version in apt is probably too old, but snap works (`sudo snap install hugo --channel=extended`)

## Download source

```
git clone --recursive git@github.com:reside-ic/naomi-news
```

## Create a new post

```
hugo new posts/<title>
```

This will create a .md file in `content/posts` which you should edit.

The front matter options that might be useful:

```
---
title: "Add a title here"
date: 2022-10-20T13:51:48+01:00
tags: ["Feature"]

hideSummary: false # set this to true to prevent the summary
summary: "A string here" # set this to force the summary content
---
```

## Writing posts

Please include a tag in your post header using `tags: ["Feature"]`. Please use one of the following tags:
* Feature - a new feature in the UI
* Update - a smaller update to something in the UI, or a less user facing update change, or a change to logic
* Model - a change to how the model works which we want to tell users about

Include a version in the header either `hint_version`, `hintr_version` or a `naomi_version`.

## Develop

If this is the first time initialise the submodules and ensure up to date

```
git submodule init
git submodule update
```

```
hugo serve
```

Visit http://localhost:1313/news/ to see changes, editing the file will reflect immediately

## Docs

* [Theme docs](https://github.com/adityatelange/hugo-PaperMod)
* [Hugo docs](https://gohugo.io/documentation/)
