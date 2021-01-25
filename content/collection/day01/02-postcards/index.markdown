---
title: "Why R Markdown?"
weight: 2
subtitle: "Why use R Markdown to introduce yourself online."
excerpt: "Of course a big plus is you can put your data science and R programming skills online, but also: you can use RStudio, and you can use tools that can help you improve your real work workflows."
date: 2021-01-25
draft: true
---

<script src="{{< blogdown/postref >}}index_files/fitvids/fitvids.min.js"></script>

## Why R Markdown?

<div class="shareagain" style="min-width:300px;margin:1em auto;">
<iframe src="/slides/02-why-rmd.html" width="400" height="300" style="border:2px solid currentColor;" loading="lazy" allowfullscreen></iframe>
<script>fitvids('.shareagain', {players: 'iframe'});</script>
</div>

## Activity

Let’s use the postcards package to make a simple postcard right now, and publish it with GitHub Pages.

### Pre-requisites

First, make sure you have the latest version of the postcards package installed from CRAN:

``` r
install.packages("postcards")
```

Restart your R session. If you use RStudio, use the menu item *Session &gt; Restart R* or the associated keyboard shortcut:

-   <kbd>Ctrl + Shift + F10</kbd> (Windows and Linux) or
-   <kbd>Command + Shift + F10<kbd> (Mac OS).

``` r
packageVersion("postcards")
[1] ‘0.2.0’
```

### Create GitHub repo

Online.

### Clone GitHub repo

``` r
usethis::create_from_github("https://github.com/apreshill/global-postcard.git")
```

:sparkles: Commit & Push! :sparkles:

You should be committing these files:

-   `*.Rproj`

-   `.gitignore`

### Create a postcard

Inside your current postcards project, use the R console:

``` r
library(postcards)
```

Then you could run (wait- don’t do this yet!):

``` r
create_postcard()
```

But you could also pick one of four templates:

1.  `"jolla"` (<https://seankross.com/postcards-templates/jolla/>) \[the default\]

2.  `"jolla-blue"` (<https://seankross.com/postcards-templates/jolla-blue/>)

3.  `"trestles"` (<https://seankross.com/postcards-templates/trestles/>)

4.  `"onofre"` (<https://seankross.com/postcards-templates/onofre/>)

``` r
create_postcard(template = "jolla") #default
create_postcard(template = "jolla-blue")
create_postcard(template = "trestles")
create_postcard(template = "onofre")
```

<aside>
Want to know more? Under the hood, these are R Markdown templates, which you can include in a package.
</aside>

### Anatomy of a postcard

YAML, body, name is index- this is special

:sparkles: Commit & Push! :sparkles:

You should be committing these files:

-   `index.Rmd`

-   `*.jpg`

But! There is no `.html` file (yet…)

### Knit the postcard

Knit button or

``` r
rmarkdown::render("index.Rmd")
```

What is new in your Git pane?

:sparkles: Commit & Push! :sparkles:

You should be committing this files:

-   `index.html`

(You may get a warning in RStudio IDE that this file is too big- go right ahead)

### Publish a postcard

Easy:

-   Push & publish to GitHub Pages: <https://docs.github.com/en/github/working-with-github-pages/creating-a-github-pages-site#creating-your-site>

Medium:

-   Use the `usethis` package to configure GitHub Pages from R:

``` r
> library(usethis)
> use_github_pages(branch = "main", path = "/")
✓ Setting active project to '/Users/alison/rscratch/global-postcard'
✓ Activating GitHub Pages for 'apreshill/global-postcard'
✓ GitHub Pages is publishing from:
● URL: 'https://apreshill.github.io/global-postcard/'
● Branch: 'main'
● Path: '/'
```

### Share your postcard!

Add it to your repository details :heart:
