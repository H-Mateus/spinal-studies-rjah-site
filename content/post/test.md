+++
title = "Writing Posts in Org using Ox-Hugo"
author = ["Gabriel Mateus Bernardo Harrington"]
date = 2019-10-13
tags = ["hugo", "org", "tools", "Emacs"]
categories = ["emacs"]
draft = false
weight = 2001
summary = "Writing hugo post in Emacs org."
+++

I use  [Emacs](https://www.gnu.org/software/emacs/emacs.html) for almost everything I do with my laptop, such as note-taking, GTD, email-checking, coding
and writing. In previous posts, I introduced some packages and my workflow in Emacs for \\(\LaTeX\\),
bibolography management and some usages Emacs as an alternative to Rstudio. In this post,
I will show how to write posts in my website in org with Hugo.


## Hugo and ox-hugo {#hugo-and-ox-hugo}

This website is built using [Hugo](https://gohugo.io/) with the [Academic Theme](https://themes.gohugo.io/academic/). I use [ox-hugo](https://ox-hugo.scripter.co/), a org exporter backend that exports Org to Hugo-compatible Markdown. To use ox-hugo,
I add the following lines in the my configuration&nbsp;[^fn:1].

[^fn:1]: In my case `init-local.el`, as I use the configuration by [Purcell](https://github.com/purcell/emacs.d).
