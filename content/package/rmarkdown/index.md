---
author: Alison Hill
categories:
- R
- package
date: "2021-01-23"
weight: 1
excerpt: The goal of the rmarkdown package is to provide output formats and tools for R users to create dynamic analysis documents that combine code, rendered output (such as figures), and prose. 
layout: single-sidebar
subtitle: "Build HTML documents, PDFs, Word files, slideshows, and websites with R Markdown."
title: R Markdown
links:
- icon: github
  icon_pack: fab
  name: code
  url: https://github.com/rstudio/rmarkdown
- icon: book
  icon_pack: fas
  name: docs
  url: https://rmarkdown.rstudio.com/
- icon: box-open
  icon_pack: fas
  name: reference
  url: https://pkgs.rstudio.com/rmarkdown/
- icon: stroopwafel
  icon_pack: fas
  name: cookbook
  url: https://bookdown.org/yihui/rmarkdown-cookbook/
---

The rmarkdown package is a single package, but "R Markdown" is the backbone for an ecosystem of packages for creating computational documents in R. In this workshop, we'll use the development version installed from GitHub.

```r
install.packages("remotes")
remotes::install_github("rstudio/rmarkdown")
```
