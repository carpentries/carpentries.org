---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: ""
title: "The Dovetail #7: Updates from The Carpentries Workbench"
date: 2022-09-21
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the seventh post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

---

We are hard at work drawing up plans for The Beta Phase, which will tentatively
restart on 2022-10-17. I have recruited members from the Curriculum, Workshop
Administration, Assessment, and Communications teams to help out with the effort.
By the time the beta phase is over and we convert our lessons (current estimate:
Q2 2023), the whole community should be aware of and excited for the changes!

In news related to the workbench, two things happened recently: 

At the beginning of September, Toby Hodges and myself hosted a short, 3 hour,
in-person workshop on developing community lessons with The Carpentries
Workbench at 
[The Conference for Research Software Engineering](https://rsecon2022.society-rse.org/). 
With over 40 attendees, it was well-attended and largely successful. There were 
a few minor hiccups that we did not anticipate, but nothing insurmoutable:

1. We had forgotten to include a live notes document at the beginning of the
   session, so sharing information (such as links for installation instructions)
   were acheived via custom `bit.ly` links.
2. Because we were working with Research Software Engineers, there was an even
   split between folks working on Windows, Mac, and Linux systems, which proved
   to be a good test for Workbench installation because, while everyone on
   Windows was able to install The Workbench successfully, folks on Linux and
   MacOS with R installed from Homebrew needed a couple of extra steps, but this
   was mitigated with the extra instructions we have in [The Workbench setup documentation](https://carpentries.github.io/sandpaper-docs/#setup)

An update to the [R for Ecologists lesson](https://carpentries-incubator.github.io/R-ecology-lesson/), which introduces data visualisation and the tidyverse first, was beta tested in a workshop. 

There are a few things to take away from this news that I find interesting:

1. We have indeed lowered the barrier for entry to work on and contribute to our
   lessons. Setup for Windows and Mac used to be very difficult, but now, with a
   default installation of R, folks are able to get setup and working right away.
   Yes, there were some extra steps required for Linux folks and Mac Homebrew
   folks, but people who have these setups tend to understand the machinery of their
   computers a lot better, making them better prepared to troubleshoot issues with installation and dependencies as they arise. 
   Furthermore, the caveats for Linux installations are [well documented in the setup](https://carpentries.github.io/sandpaper-docs/index.html#linux). 
2. The fact that The R for Ecologists lesson was tested in a workshop recently
   and I did not receive critical feedback about it means that either of these can be true:
   a) our community is very resilient to change and b) Even though The Workbench
   approaches lessons with a different design, navigating the new layout is
   understandable and useable enough that there were no noticable issues during
   live instruction or preparation.

## Updates to The Carpentries Workbench

Since 2022-08-24, 

The Markdown parser, [{tinkr}](https://cran.r-project.org/package=tinkr) has
been released on CRAN!

 - [{sandpaper} version 0.9.3 -> **0.10.0**](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0100)
   - Minor maintenance fixes
   - `create_episode()` and variants will now default to creating episode names _without_ a prefix and will update the lesson schedule. You can insert the episode to a specific place in the schedule by using the add parameter (e.g. `add = 2` will place the episode in the second position). 
   - **NEW** `draft_episode()` variants will create an episode, but not insert it into the schedule.
   - **NEW** `move_episode()` allows you to move a single episode or draft to a different part of the schedule programmatically or interactively.
   - **NEW** helper function `strip_prefix()` will strip the numeric prefix of your existing episodes and add them to the schedule in the correct order (NOTE: this will cause existing links to become invalid, so be prepared to correct those).
   - A small bug fix where some anchor links in callouts were `NA` was fixed.
 - [{pegboard} 0.3.1 -> 0.3.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-032)
   - Maintenance fix for an updated version of the [{cli} package](https://cran.r-project.org/package=cli)
   - Unused soft dependencies have been dropped
 - [{varnish} 0.2.4](https://carpentries.github.io/varnish/news/index.html#varnish-024)
   - no updates :)

To update your local Workbench installation, open R and use the following code:

```r
# Enable repository from carpentries
options(repos = c(
  ropensci = 'https://carpentries.r-universe.dev',
  CRAN = 'https://cloud.r-project.org'))
# Download and install sandpaper in R
install.packages(c('tinkr', 'pegboard', 'sandpaper', 'varnish'))
```

## Upcoming and Current Lessons in Workbench Beta

### List of Lessons to enter Workbench Beta in 2022

#### Official Lessons

 - [datacarpentry/R-ecology-lesson---Data Analysis and Visualization in R for Ecologists](https://github.com/datacarpentry/R-ecology-lesson/discussions/799) (✅ approved by maintainers)
 - [datacarpentry/r-socialsci---R for Social Scientists](https://github.com/datacarpentry/r-socialsci) (✅ approved by maintainer)
 - [datacarpentry/r-raster-vector-geospatial---Introduction to Geospatial Raster and Vector Data with R](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/369) (⏳ awaiting responses)
 - [datacarpentry/OpenRefine-ecology-lesson---Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson) (✅ approved by maintainer)
 - [librarycarpentry/lc-shell---Library Carpentry: The UNIX Shell](https://github.com/librarycarpentry/lc-shell) (⏳ awaiting responses)
 - [carpentries/instructor-training---Instructor Training](https://github.com/carpentries/instructor-training) (⏳ awaiting responses)

##### Tentative schedule for official lessons

**[ON HOLD]**

#### Community Lessons

 - [carpentries-incubator/git-novice-branch-pr---Version Control with Git](https://github.com/carpentries-incubator/git-novice-branch-pr)
 - [carpentries-incubator/data-management-pipelines-engineering---Data management and analytic pipelines for engineers](https://github.com/carpentries-incubator/data-management-pipelines-engineering)
 - [carpentries-incubator/markdown-intro---Introduction to Markdown](https://github.com/carpentries-incubator/markdown-intro)
 - [carpentries-incubator/SDC-BIDS-IntroMRI---Introduction to MRI and BIDS](https://github.com/carpentries-incubator/SDC-BIDS-IntroMRI)
 - [carpentries-incubator/SDC-BIDS-dMRI---Introduction to dMRI](https://github.com/carpentries-incubator/SDC-BIDS-dMRI)
 - [carpentries-incubator/SDC-BIDS-fMRI---fMRI Imaging Analysis](https://github.com/carpentries-incubator/SDC-BIDS-fMRI)
 - [carpentries-incubator/julia-novice---A lesson exploring the Julia language](https://github.com/carpentries-incubator/julia-novice)
 - [carpentries-incubator/R-archaeology-lesson](https://github.com/carpentries-incubator/R-archaeology-lesson/issues/4#issuecomment-1138641684)
 - [carpentries-incubator/python-packaging-publishing---Packaging and Publishing with Python](https://github.com/carpentries-incubator/python-packaging-publishing)

### Participants

 - Eirini Zormpa, Maintainer
 - James Sadler, Maintainer
 - [Robin](https://github.com/longr/), Instructor
 - [Jon Haitz Legarreta Gorroño](https://github.com/jhlegarreta/), Lesson Developer (in The Carpentries Incubator)
 - [Karen Word](https://github.com/karenword/), Maintainer
 - [Luis J. Villanueva](https://github.com/villanueval/), Maintainer
 - [Jon Wheeler](https://github.com/jonathanwheeler01/), Lesson Developer (in The Carpentries Incubator)
 - Simon Christ, Lesson Developer (in The Carpentries Incubator)
 - [Maneesha Sane](https://github.com/maneesha/), Instructor
 - [Sarah Brown](https://github.com/brownsarahm/), Maintainer
 - [Joel Nitta](https://github.com/joel.nitta/), Translator
 - [Juan Fung](https://github.com/juanfung/), Maintainer
 - [Jannetta Steyn](https://github.com/jsteyn/), Lesson Developer (in The Carpentries Incubator)
 - [Michael Joseph](https://github.com/josephmje/), Lesson Developer (in The Carpentries Incubator)
 - [Sarah Stevens](https://github.com/sstevens2/), Lesson Developer (in The Carpentries Incubator)
 - [Kozo Nishida](https://github.com/kozo2/), Lesson Translation (to Japanese)
 - François Michonneau, Maintainer
 - [Jamie Jamison](https://github.com/jmjamison/), Maintainer
 - Jennifer Stubbs (she/her), Instructor
 - [Drake Asberry](https://github.com/drakeasberry/), Maintainer

## Tips and Tricks for Using The Workbench

**If you use Linux or Homebrew with MacOS** and you want to install The
Workbench locally, you should read some of the caveats in
[the workbench setup instructions for Linux](https://carpentries.github.io/sandpaper-docs/index.html#linux).

For most users R's package management system _just works_. If you want a package,
you can install it with the R command `install.packages("<package-name>")` and 
R will search available repositories for the package and install it. 

The reason why this works is because R's default repository,
[CRAN](https://cran.r-project.org) hosts pre-built binary versions of these
packages for Windows and MacOS[^1]. This means if you are a user of one of these
systems and you need to install an R package that uses C code behind the scenes,
you do not need a compiler in order to use that package because the code is
already compiled and ready to use.

For Linux and Homebrew MacOS systems, the toolchain for compilation is variable
enough that it is not feasible for a global archive network to compile binaries
for all the possible Linux and Homebrew variants, so you get the source code for
the packages and must compile them yourself. 

If you find yourself in this situation, know that there are some external C 
libraries that you need to install. Error messages will let you know what
libraries you need, but the R-universe provides [a handy list of the 
requirements through its API](https://carpentries.r-universe.dev/stats/sysdeps),
which you can query using curl to install:

```r
curl https://carpentries.r-universe.dev/stats/sysdeps 2> /dev/null \
| jq -r '.packages[0] | select(. != null)'
```

```
libcurl4-openssl-dev
libfontconfig-dev
libfreetype-dev
libfribidi-dev
libharfbuzz-dev
libicu-dev
libgit2-dev
libjpeg-turbo8-dev
libpng-dev
libtiff-dev
libxml2-dev
libxslt1-dev
libssl-dev
```


[^1]: The Workbench is hosted on <https://carpentries.r-universe.dev/> and not
  CRAN because the R-Universe allows for rapid patch fixes and updates, 
  making it better-suited to newer packages that are under active development and may change frequently,
  whereas CRAN's policies expect updates on a 2-month cycle. 
