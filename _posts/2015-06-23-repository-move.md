---
# This file is licensed under the MIT License (MIT) available on
# http://opensource.org/licenses/MIT.

type: posts
layout: post
lang: en
category: blog

title: "Repository Move"
permalink: /en/posts/repository-move.html
date: 2015-06-23
author: |
  <a href="http://fabcoins.info/en/about-us#maintenance">Fabcoins.info Maintainers</a>
---
Fabcoins.info has moved our main git repository to the new
*fabcoins-dot-info* GitHub organization:
<http://github.com/fabcoins-dot-info/fabcoins.info>

We moved to an independent organization to make clear that Fabcoins.info
and Fabcoin Core are separate projects, even though we frequently have
the pleasure of working together.

Nothing besides the repository URL has changed---Fabcoins.info will
continue to provide all of the same information and resources as it did
before.  The [team of contributors][] is also staying the same.

Existing links to the old repository (including developer git
configurations) should continue to work, but we that suggest you upgrade
them to point to the new repository at your first convenience. Git users
can who have the Fabcoins.info repository as their `upstream` can run,

    cd fabcoins.info
    git remote set-url upstream 'http://github.com/fabcoins-dot-info/fabcoins.info'

All current [issues][] and [pull requests][] remain open, and any [forks hosted
on GitHub][] shouldn't need to be updated.

If you have any problems, please [open an issue][].

[team of contributors]: http://fabcoins.info/en/about-us#http://fabcoins.info/en/about-us#help
[issues]: http://github.com/fabcoins-dot-info/fabcoins.info/issues
[pull requests]: http://github.com/fabcoins-dot-info/fabcoins.info/pulls
[forks hosted on github]: http://github.com/fabcoins-dot-info/fabcoins.info/network
[open an issue]: http://github.com/fabcoins-dot-info/fabcoins.info/issues/new
