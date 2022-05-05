# statements-on-tools
The NHS-R Community statements on the use of tools including (but not excluding) R and R Studio. 

# Introduction

R uses **packages**. Packages are small, reusable packages of code that allow users to create and use new functions. These packages can be easily distributed so that users can adapt

<!-- Packages are a way of distributing code.  -->

Imagine that you are writing some code, and run into a slightly tricky problem. The traditional approach would be to write new code yourself from scratch that resolves the problem. But very often, the problems that we encounter are not unique, but are the kind of thing that others might have encountered many times before. So writing new code each time is wasteful. 

That said, finding and sharing functional code to solve common problems is not easy. You could look for solutions online using sites like [StackOverflow](https://stackoverflow.com/), and then copy and paste any promising code chunks into your project. But that process is messy - it requires you to have an expert's eye for assessing possible solutions, and then the skills to carefully adjust borrowed code to fit the requirements of your project.

Packages are a way of standardising and sharing useful code. Rather than copying and adjusting a block of code, you simply add the package to your programme, and then use the new functions that are contained in the package. Many programming languages use packages (or libraries) in a similar way. Python is a good example, where many useful functions are done using third-party packages.

Packages make R better: easier to use and learn, more flexible, and with richer options for analysis. They are a feature and not a bug.

The power of packages is reflected in the number of them that are available. CRAN (the [Comprehensive R Archive Network](https://cran.r-project.org/)) currently lists a total of 18872 packages. Adding and updating packages is one of the ways that R keeps developing. Many community groups - including [NHS-R](https://nhsrcommunity.com/about) - have produced packages to do useful things for their work. And these packages are freely available to the community.

(something something open source software)
(Might be nice to have a greatest hits box of links here)

That community spirit is an important part of the open software movement. We think that sharing useful code in an open way is important. Governments too think similarly. For example, see the requirement to make new code open source from [NHS England digital openness](https://service-manual.nhs.uk/standards-and-technology/service-standard-points/12-make-new-source-code-open) and similar from ScotGov. The recent Goldacre review (2022) comes to similar conclusions:

>**Libraries**
Useful functions often outgrow individual projects and build a broader user-base, especially when a large number of users are all trying to solve the same suite of related problems, with a range of related functions. When this happens, more experienced programmers move the work into reusable code ‘libraries’ and share them through package indexes or archive networks. The process of creating and sharing libraries can improve the quality of code, because work that is more widely used is likely to be more widely reviewed. Popular libraries tend to be well documented and come with clear explanations and examples, which decrease the barriers to entry for inexperienced coders: when more people use the work, more people invest in improving it. By creating and sharing a library, researchers contribute to the broader research community. This more advanced variety of code sharing is common in many areas of scientific research, such as Geographic Information Science, but it is less common at present in health data research.

[Better, broader, safer: using health data for research and analysis](https://www.gov.uk/government/publications/better-broader-safer-using-health-data-for-research-and-analysis/better-broader-safer-using-health-data-for-research-and-analysis#information-governance-ethics-and-participation)

Safe, too: R hasn't had any bugs or problems that could cause any security issues

## An example
For example, working with dates is often a source of pain for data analysts. That's because dates are complicated. For example, there are lots of ways of storing and representing dates. There are also many inconsistencies - 24 hours in a day but 60 seconds in a minute, leap years, different numbers of days in months, time zones, and so on.

Many analysts use an R package called [lubridate](https://lubridate.tidyverse.org/) to help manage dates and times. This package has lots of helpful functions for parsing, calculating, and representing dates and times. For example, imagine that you want to calculate the number of seconds between two dates. For simple cases, that's not too hard to do in base R. But what if some of your time values cross time zones? What if the clocks changed (say, due to daylight savings) during that interval? The functions in the lubridate package allow analysts to ignore some of this complexity, meaning that they don't need to write many lines of code in order to accomodate time zones each time they want to do a simple duration calculation.

# What's the problem

+ Something of a moving target for information governance.
+ Rapid change and large numbers of packages (c.19k packages on CRAN)
+ Confusion between data and software
+ Apparent credibility of (F)OSS
+ Multiple sources for packages (CRAN, GitHub, ...)
+ Community oversight for package standards

Useful comments in FAQ section of [https://sites.google.com/nihr.ac.uk/hsma/apply-to-become-an-hsma?authuser=0](HSMA) site:

>It is also important to highlight that all software has potential vulnerabilities, including the proprietary software that you already have installed. Therefore, good software security practices should be maintained regardless of the software you are using.

# Contributors
Produced by the NHS-R community with the contributions of Zoe Turner, Dr Daniel Chalk, and Brendan Clarke
