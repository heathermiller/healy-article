## healy-article

This repository contains the minumum that you need to create LaTeX articles
beautifully typeset using one of [Kieran Healy](http://kieranhealy.org/)'s
[excellent LaTeX templates](https://github.com/kjhealy/latex-custom-kjh).

**Example:**

![](https://raw.githubusercontent.com/heathermiller/healy-article/master/page-thumbnail.png)

This version builds slightly on Kieran's template by merely including the
[minted package](https://github.com/gpoore/minted) for beautiful source code
highlighting and formatting.

### Why this repo?

This repo serves only to provide a minimum working version of Kieran's basic
article template with LaTeX alone. It took me a while to be able to build this
template on my machine, so I  created this repository for those who simply want
to get up and running quickly without needing to involve pandoc, R, etc.

Just make sure you have the basic dependencies, check out the repo, and build.

### Dependencies

1. A standard TeX Live distribution.
  - For OS X there's [MacTeX](http://tug.org/mactex/)
  - For Linux and Windows, there's [TeX Live](http://www.tug.org/texlive/)
2. [Pygments](http://pygments.org/), an automatic syntax highligher
  - Assuming that Python is already installed on your system, to install Pygments, simply run:

    `sudo easy_install Pygments`
(If you already have pygments and you get any latex errors that say anything about `out.pyg` files, just run the above to update pygments)
3. Minion Pro and Consolas fonts, installed system-wide. All required fonts can be found in `fonts` directory, just install.

### Building

Assuming your tex file is named `healy-article.tex` as it is in this repo,
simply run:

    xelatex --shell-escape healy-article
