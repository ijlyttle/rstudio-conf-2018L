---
title: "How I Learned to Stop Worrying and Love the Firewall"
author: Ian Lyttle, Schneider Electric
bibliography: references.bib
---

## Abstract

R's open-source communities have built robust package-frameworks that "just work". CRAN is a well-celebrated example;
__devtools__ [@R-devtools] makes it easier for us to install and develop packages using public GitHub repositories. RStudio Connect and its underlying packages, __rsconnect__ [@R-rsconnect]  and __packrat__ [@R-packrat], work intuitively if all the packages you use are on either CRAN or public GitHub. However, if you are working in a corporate environment to develop private packages, this is no longer the case. I will present a set of workarounds that work well for me: using __devtools__ to develop and deploy packages on GitHub Enterprise, and using __drat__ [@R-drat] to maintain a CRAN-like repository within our firewall. I will show how I use these tools to deploy private packages to our instance of RStudio Connect, as well as to cloud VMs outside our firewall. 

