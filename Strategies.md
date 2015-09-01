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

If you have a topic that requires both text AND code, then you can combine both strategies. You store code, data, resources, and instructions in the `master` branch of the repo and you store HTML, CSS, and Javascript in the repo on the `gh-pages` branch.

To take advantage of this approach, follow these (high-level) steps:

1. create a new repo and associate it with GitHub
2. on the `master` branch, fill it with code and markdown files
3. `git checkout -b gh-pages`
4. `git rm <everything>`; `git commit`
5. Now, fill the `gh-pages` branch with HTML, CSS, and Javascript
6. Switch between the two branches to work on code (`master`) and your website (`gh-pages`) until done
7. `git push` frequently to view repo/website as it evolves on GitHub

Note: step 4 creates an empty working directory on the gh-pages branch. It will consist of multiple calls to the `git rm` command until everything in the working directory has been deleted, followed by a `git commit` to give the `gh-pages` branch a new starting point.

This might seem scary, but it's not. All of those files are safe on the `master` branch. Just enter `git checkout master` to see them again and then `git checkout gh-pages` to go back to the empty directory so you can start working on your website.

## Examples

I have created two examples to view associated with my Github account.

The first is this lecture presented with Markdown files on the master branch of this repository. (You're looking at it now!)

Option 1: https://github.com/kenbod/markdown_github_01

The second is this lecture presented, again, as a website on the gh-pages branch of the same repository.

Option 2: https://kenbod.github.io/markdown_github_01

A <q>code heavy</q> example is left as an exercise for the reader.

## Next Steps

Next up, head to the [Wrapping Up](https://github.com/kenbod/markdown_github_01/blob/master/Strategies.md) page or
head back to the [Table of Contents](https://github.com/kenbod/markdown_github_01/blob/master/README.md).

