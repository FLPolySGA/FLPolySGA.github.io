---
layout: page
title: "README"
permalink: /README
toc: true
---

[**VISIT THE LIVE PAGE**](https://flpolysga.github.io)

[**VIEW THE README ON THE WEBSITE**](https://flpolysga.github.io/README)

## Table of Contents

- [About Our Website](##About-Our-Website)
- [Contributing](#Contributing)
- [Creating a Local Copy](##Creating-a-Local-Copy)
  - [Cloning the Repository](###Cloning-the-Repository)
  - [Installing Jekyll](###Installing-Jekyll)
  - [Running a Local Copy](###Running-a-Local-Copy)

## About Our Website

### Basics

Our website is written in [markdown](https://www.markdownguide.org/getting-started/) and hosted on [GitHub pages](https://pages.github.com). The heavy lifting to turn the markdown into a fully-fledged website is done through [Jekyll](https://jekyllrb.com) with the conversion happening with [GitHub actions](https://github.com/features/actions).

### Workflow

1. Someone submits a pull request with new changes

2. The Director of Standards and Enforcement reviews the changes and chooses to either deny the pull request or approves and merges it into `main`. Changes should not be made directly on `main`.

3. When GitHub actions detects changes on `main`, the live site is built on `gh-pages`

   > DO NOT INTERACT WITH THE `gh-pages` BRANCH

4. The site may take a few minutes to build and go live

   > If the build fails, the old site will remain. If the build succeeds with errors, work quickly to recover the old site and correct the errors before trying again.

## Contributing

### Using Markdown

- A basic guide for using mardown can be found [here](https://www.markdownguide.org/basic-syntax/). If you would like to see the source code for this page and what it looks like behind the scenes, you can view it [here](https://raw.githubusercontent.com/FLPolySGA/FLPolySGA.github.io/main/README).

### Creating a Pull Request

- GitHub has instructions on creating a pull request [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

### Being Added as a Contributor

- If you are in a position where you feel it is appropriate to be added as a contributor, contact the Director of Standards and Enforcement. Their contact info can be found on the [Meet Executive](https://flpolysga.github.io/AboutSGA/MeetExecutive/) page.

## Creating a Local Copy

### Cloning the Repository

#### GitHub Desktop (Recommended)

1. Download and install GitHub Desktop from [their download page](https://desktop.github.com)
2. There are three ways to clone the repo
   - Visit [the repo](https://github.com/FLPolySGA/FLPolySGA.github.io) and click `Code`, then `Open with GitHub Desktop`
   - Click this link to perform the same action directly <a href="x-github-client://openRepo/https://github.com/FLPolySGA/FLPolySGA.github.io">here</a>
   - Open GitHub Desktop and click `Add`, then `URL` and enter `FLPolySGA/FLPolySGA.github.io`

#### Command Line Interface

1. Follow GitHub’s instructions on installing their CLI [here](https://cli.github.com)
2. Run `gh repo clone FLPolySGA/FLPolySGA.github.io` in your terminal

### Installing Jekyll

> This does not always go smoothly and may take a few tries!

1. Follow the instructions on Jekyll’s website [here](https://jekyllrb.com/docs/)

### Running a Local Copy

1. Open terminal and change directories to your local repository’s root folder
2. There are two ways to run the site
   - To run a live reload version (recommended, but more prone to issues), run <br>`bundle exec jekyll serve --livereload`
   - To run a static version, run `bundle exec jekyll serve`