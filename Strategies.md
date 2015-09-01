# Strategies for Using GitHub Presentations

## Overview

There are three basic approaches for creating your presentations in GitHub.

1. Create a repo that contains both code and Markdown files. The Markdown files act as your presentation.
2. Create a repo that uses the `gh-pages` branch to create a website that GitHub serves
3. Create a repo with both code and Markdown files in the `master` branch and a website in the `gh-pages` branch

## Option 1: Markdown/Code in `master` branch

If you pick a topic that requires writing a lot of code, then you can use `git` to create a repo with a `master` branch. Your repo would have a top-level directory that contained a `README.md` file, a `src` directory and a `docs` directory to contain a Markdown-based presentation. You might have other top level directories that contain data, resources, and other information (such as installation instructions).

Say you decided to do a presentation on _Functional Programming in Scala_ and how Scala and the functional programming paradigm can help software engineers write better code. You can create sub-directories under the `src` directory for each of your Scala-based examples. You can create a set of Markdown files in the `docs` directory that presents your information on Scala and functional program and uses Markdown code-blocks to present your Scala code examples. Your `README.md` might then contain pointers and instructions on how to install Scala and how to run the various code examples.

You would have your repo on your local machine and on GitHub. You might work on the code on your machine and do frequent commits and uploads to GitHub (via `git push`). You might then switch to working on the Markdown using GitHub's markdown editor, making frequent commits on-line. You would then update your local repo with `git pull` to keep it consistent.

## Option 2: Website in `gh-pages` branch

If your presentation has no code but lots of text and images, then you can create a repo that takes advantage of GitHub's ability to associate a website with a given repo.

To take advantage of this functionality, follow these (high-level) steps:

* create a new repo and associate it with GitHub
* `git checkout -b gh-pages` (you will never use the `master` branch again)
* add HTML, CSS, and Javascript to your repo
* `git push -u origin gh-pages`

If your repo is stored at

    https://github.com/<USER>/<REPO>

then your website will automatically appear at 

    https://<USER>.github.io/<REPO>/

I did this last year for one of my seminars:

* Repo: <https://github.com/cu-data-engineering-s15/lecture_05>
* Website: <https://cu-data-engineering-s15.github.io/lecture_05/>

## Option 3: Why not Both?
