---
title: "Prework"
weight: 1
subtitle: ""
excerpt: "Grid is the very first CSS module created specifically to solve the layout problems we’ve all been hacking our way around for as long as we’ve been making websites."
date: 2021-01-01
draft: false
---

{{< here >}}


Welcome to the [Communicating with R Markdown](/) workshop! We look forward to meeting you in person. Before attending the workshop, please complete the following prework:

1. Sign up for a free RStudio Cloud account at https://rstudio.cloud/ before the workshop. I recommend logging in with an existing Google or GitHub account, if you have one (rather than creating a new account with another password you have to remember).

1. We will be using GitHub in this workshop for version control and publishing. Sign up for a free GitHub.com account at <https://github.com/join> if you don't already have one. Also:

    + Complete these [installation instructions](https://happygitwithr.com/install-intro.html).
    
    + Test your connection between GitHub and RStudio following [these steps](https://happygitwithr.com/connect-intro.html). 
    
    + **NOTE:** We *strongly recommend* that if you are not already a fluent GitHub user you choose [HTTPS over SSH](https://happygitwithr.com/credential-caching.html).

1. Complete this [10-minute interactive tutorial on Markdown](https://commonmark.org/help/tutorial/). 

1. Please bring a laptop that has the following installed:

    + A recent version of R (>=3.6.0), which is available for free at https://cloud.r-project.org/
    
    + A recent version of RStudio Desktop (>=1.2), available for free ([RStudio Desktop Open Source License](https://www.rstudio.com/products/rstudio/download/#download))
    
    + The R packages we will use, which you can install by connecting to the internet, opening RStudio, and running at the command line:

        ```{r pkg-list, eval=FALSE}
        install.packages(c("rmarkdown", "devtools", "usethis", "here", 
                           "tidyverse", "xaringan", "flexdashboard", 
                           "distill", "bookdown", "blogdown",
                           "glue", "wesanderson"))
        ```
    
1. Don't forget your power cord!

On the day of the workshop, I'll provide you with an RStudio Cloud project that contains all of the course materials. We will use the software listed above only as an important backup should there be problems with the on-site internet connection.
