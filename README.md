# README

This is the website of the RAPID-CDL project.



# Editing workflow

## Setup

You'll need to install:

- quarto
- git


## Where to put things

Quarto is configured to render all .qmd files automatically.

Pages (index.qmd, about.qmd) are kept at the top level - we shouldn't need too many of these.

Blog posts go in the `blog/posts` folder - you can create a new folder, or for simple text only posts just a new file at the top level.


## Blog Post Details

You'll need YAML metadata like the below for the blog post to render in the blog listing page, otherwise standard markdown is fine.

```
---
title: "Welcome To My Blog"
author: "Tristan O'Malley"
date: "2026-02-22"
categories: [news]
---

``` 


## Editing and Pushing Changes

Important: the `docs/` folder is what the live site will look like when pushed to github!

The edit workflow is:

1. Make changes to the source files (.qmd/.md)
2. Render the changes with `quarto render` to render everything, or `quarto render path/to/file` for just the one.
3. Preview changes by opening the output files (built into the `docs` folder)
4. Use git to add, commit and push changes. You need to commit both the edited source files, and also the rendered outputs in the docs/ folder.
