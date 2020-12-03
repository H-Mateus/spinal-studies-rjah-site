+++
title = "Org-mode basics"
author = ["Gabriel Mateus Bernardo Harrington"]
date = 2020-12-03
tags = ["Emacs", "org", "tools"]
categories = ["emacs"]
draft = false
weight = 2002
summary = "Brief introduction to org-mode formatting"
+++

This is a brief introduction to formatting in [org-mode](https://orgmode.org/) made mostly to help my dear colleagues with writing content for the site


## Why org-mode? {#why-org-mode}

This website uses a single [org-mode](https://orgmode.org/) file to manage most of the content.
Org-mode is an example of a [markup language](https://en.wikipedia.org/wiki/Markup%5Flanguage), which means the text formating is described in the text itself.
This is in contrast to a "[what you see is what you get](https://en.wikipedia.org/wiki/WYSIWYG)" system where the formatting information is hidden from the user and stored in the file data somehow, as Microsoft Word does with it's proprietary file formats.

There are several advantages to using plain text.
Perhaps the most important of which is transportability and reproducibility.
You can't view or edit a .doc file without special software (which you often have to pay for), whereas plain text files can be viewed an edited on any computer, regardless of operating system, and with thousands of text editors to choose from.

The only real disadvantage to markup languages is that you have to learn their syntax.
This is only really an issue for some languages though, [html](https://en.wikipedia.org/wiki/HTML#:~:text=Hypertext%20Markup%20Language%20(HTML)%20is,scripting%20languages%20such%20as%20JavaScript.) (the language website are written in) is fairly complicated and fiddly, but languages like [markdown](https://en.wikipedia.org/wiki/Markdown#:~:text=Markdown%20is%20a%20lightweight%20markup,Markdown) and org-mode where made to be simple and easy to learn.

And this post is going to teach the basics, so read on!


## Formatting {#formatting}

For example, if you would like **bold text**, you simply wrap the text with \* like so: `*bold*`
similarly, we can have

<div class="table-caption">
  <span class="table-number">Table 1</span>:
  If you're wondering how I'm able to show the formatting without it rendering have a look at the .org file on the
</div>

| Rendered text                             | Raw text           |
|-------------------------------------------|--------------------|
| _italics_                                 | `/italics/`        |
| `monospace`                               | `=monospace=`      |
| `code`                                    | `~code~`           |
| ~~strike-through~~                        | `+strike-through+` |
| <span class="underline">underlined</span> | `_underlined_`     |


## Headings {#headings}

For headings org-mode uses \*:

-   `* Level one header`
-   `** Level two header`
-   `*** Level three header`

and so on. Org-mode will automatically scale the text to the size of the level of the header.


## Links and images {#links-and-images}

To insert [links](https://en.wikipedia.org/wiki/Hyperlink) use square brackets like so: `[[link_address_goes_here][text_goes_here]]`
The link in the previous sentence looks like this:
`[[https://en.wikipedia.org/wiki/Hyperlink][links]]`

To insert images we do the same, but the link has to point to an image.
So `[[file:red_panda.jpg]]`
Results in the following image being embedded
![](/ox-hugo/red_panda.jpg)
