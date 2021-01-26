---
title: "Why Netlify?"
author: Alison Hill
weight: 5
subtitle: "Using Netlify to build websites in the cloud."
date: 2021-01-26
draft: false
links:
- icon: campground
  icon_pack: fas
  name: slides
  url: "/slides/05-why-netlify.html"
- icon: hiking
  icon_pack: fas
  name: activity
  url: "collection/day02/05-netlify/#activity"
---

<script src="{{< blogdown/postref >}}index_files/fitvids/fitvids.min.js"></script>

## Why Netlify?

<div class="shareagain" style="min-width:300px;margin:1em auto;">
<iframe src="/slides/05-why-netlify.html" width="1600" height="900" style="border:2px solid currentColor;" loading="lazy" allowfullscreen></iframe>
<script>fitvids('.shareagain', {players: 'iframe'});</script>
</div>

## Activity

TIME: ⏱ 10 minutes

Go to this repo:
<https://github.com/apreshill/iyo-apero>

Click on the “Deploy to Netlify” button 🚀

### Clone GitHub repo

We just created:

-   a full blogdown project…
-   containing a Hugo site…
-   deployed to Netlify…
-   in a remote repository on YOUR GitHub (i.e., `https://github.com/<you>/iyo-apero`; you may have changed the repo name after clicking on the “Deploy to Netlify” button).

To make a local copy on our computer that we can actually work in, we’ll clone that repository into a new RStudio project. This will allow us to sync between the two locations: your remote (the one you see on github.com, and the one continuously deployed by Netlify) and your local desktop.

Use the RStudio IDE project wizard:

1.  Open up RStudio to create a new project where your website’s files will live.

2.  Click `File > New Project > Version Control > Git`.

3.  Paste the URL from GitHub (either HTTPS or SSH)

4.  Be intentional about where you tell RStudio to create this new Project on your workstation.

5.  Click Create Project.

**Alternatively**, do this (but note that it requires a [GitHub personal access token](https://happygitwithr.com/credential-caching.html#get-a-pat)):

``` r
usethis::create_from_github("apreshill/iyo-apero", 
                            destdir = "/Users/alison/rscratch",
                            fork = FALSE)
```

### Serve your site locally

Use the serve site add-in from the blogdown package to preview your site:

![](addin-serve-site.png)

You should be **all set** to now commit / push / pull from your *personal* GitHub repository freely! Every commit to the `main` branch will trigger your Hugo site to be built and deployed again via Netlify :magic:

### File scavenger hunt

You have 10 minutes to get to know this new Hugo site.

How? Meet the here bot! :mag:

Try to use the here bot messages to find the content file that produces the content in this starter site. There are:

-   3 blog posts
-   3 projects
-   3 talks

There are also 3 kinds of “layouts”:

-   Single
-   Single sidebar
-   Single series

See if you can spot all of these! Think of it like an easter egg hunt :egg:
