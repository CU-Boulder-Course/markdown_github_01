# GitHub

![Octocat](https://github.com/kenbod/markdown_github_01/blob/master/resources/Octocat.png "GitHub's Mascot")

GitHub is a Web-based repository hosting service for `git`. You can upload your repositories to it and then
access/manipulate them with a nice Web-based interface for many of the most common `git` commands. You
can create as many public repositories as you want; you have to pay if you want to keep your repositories private.
GitHub then adds new services on top of `git` that are designed for collaboration:

* access control
* issue tracking
* notifications
* pull requests

## Brief Introduction

I will not attempt to present a comprehensive introduction to GitHub. Features that I don't cover can become the topic of YOUR presentations :smiley:. Take a look at <https://github.com/features> for more info.

Instead, I plan to cover:

* how you can use GitHub as a remote copy of a local repository which will let us explore the `git pull` and `git push` commands
* how you can use GitHub to serve your presentations to the world (you're looking at one such use now!)

## Assumptions

I assume that you:

* have a GitHub account
    * you will need one for this class; so please create one, if needed!
* have followed the <q>[Set Up Git](https://help.github.com/articles/set-up-git/)</q> instructions at [GitHub Bootcamp](https://help.github.com/categories/bootcamp/)
* have configured your account to avoid having to type your password each time you access your remote repository from the command line
    * When you issue `git clone`, `git fetch`, `git pull`, and `git push` requests, GitHub will ask you for your password or passphrase
    * If you don’t want to type that each time, you will need to
        1. [create/upload your public key file to your GitHub profile](https://help.github.com/articles/generating-ssh-keys/), or
        2. store your [GitHub password in a credential helper](https://help.github.com/articles/caching-your-github-password-in-git/)

# Linking Repositories

The first thing that needs to happen to work with Github is linking a repository on your computer to one that exists on Github. There are two primary ways to do this.

1. If the repo exists on GitHub and not on your computer, use the `git clone` command.
2. If the repo exists on your computer but not on GitHub, then create an empty repo on GitHub and then upload your repo to it.

Let's explore both of these scenarios.

## Using the `git clone` command

If the repo exists on GitHub already, then go to the repository's page on GitHub and look for the `SSH clone URL`


