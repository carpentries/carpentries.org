---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Dates for Beta Phase Announced"
title: "The Dovetail #8: Updates from The Carpentries Workbench"
date: 2022-10-05
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the eighth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

---

## Beta Phase To Resume

As we enter into the Q4, I am pleased to announce that the long-delayed beta
phase will commence from 2022-10-17 until 2023-03-13 with one lesson entering
the beta phase per week. Details of the beta phase and the official table of
lessons can be found below and [on the Workbench Beta Phase page](https://carpentries.github.io/workbench/beta-phase.html),
with explanation of what the different stages of the beta phase will bring.

In brief, the beta phase will run for 12 weeks[^weeks] for each lesson during 
which a link will appear on the lesson, leading to the same lesson using The
Carpentries Workbench. During the beta phase, **we will be asking for feedback
about your experience with The Workbench in short assessments** and will then invite
participants to an optional focus group to gather qualitative feedback. The
feedback we receive from the assessments and focus group will make sure that The Workbench
rollout in 2023-Q2 is smooth. 

I will be recording a short video to be distributed next week (and with the next 
edition of The Dovetail) that will introduce the beta phase and demonstrate what
you can expect to see during that phase.

[^weeks]: because this version of the beta phase passes through the last week of December and the first week of January, each lesson's beta phase will be extended by two weeks for a total of 14 weeks, assuming 2 weeks of down time for lesson maintainers.

## Updates to The Carpentries Workbench

Since 2022-09-28, 

 - [{sandpaper} version 0.10.0 -> 0.10.1](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0101)
   - Titles inserted into `index.md` will replace "Summary and Setup". 
 - [{pegboard} 0.3.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-032)
   - no updates :)
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

| Lesson                                                   | Pre-Beta   | Beta       | Pre-release |
| -------------------------------------------------------- | ---------- | ---------- | ----------- |
| [datacarpentry/R-ecology-lesson---Data Analysis and Visualization in R for Ecologists](https://github.com/datacarpentry/R-ecology-lesson/discussions/799) (✅ approved by maintainers)      | 2022-10-17 | 2022-11-14 | 2023-01-23  |
| [datacarpentry/r-socialsci---R for Social Scientists](https://github.com/datacarpentry/r-socialsci) (✅ approved by maintainer) | 2022-10-24 | 2022-11-21 | 2023-01-30  |
| [datacarpentry/r-raster-vector-geospatial---Introduction to Geospatial Raster and Vector Data with R](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/369) (⏳ awaiting responses) | 2022-10-31 | 2022-11-28 | 2023-02-06  |
| [datacarpentry/OpenRefine-ecology-lesson---Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson) (✅ approved by maintainer) | 2022-11-07 | 2022-12-05 | 2023-02-13  |
| [librarycarpentry/lc-shell---Library Carpentry: The UNIX Shell](https://github.com/librarycarpentry/lc-shell) (⏳ awaiting responses) | 2022-11-14 | 2022-12-12 | 2023-02-20  |
| [carpentries/instructor-training---Instructor Training](https://github.com/carpentries/instructor-training/issues/1396) (⏳ awaiting responses) | 2022-11-28 | 2023-01-09 | 2023-03-06  |
| [datacarpentry/python-ecology-lesson-es---Análisis y visualización de datos usando Python](https://github.com/datacarpentry/python-ecology-lesson-es) | 2022-12-05 | 2023-01-16 | 2023-03-13  |


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

 - [Sara Morsy](https://github.com/https://github.com/SaraMorsy/), Lesson Developer (in The Carpentries Incubator)
 - [@iramosp](https://github.com/iramosp), Maintainer
 - [Jesse Sadler](https://github.com/jessesadler/), Maintainer
 - Eirini Zormpa, Maintainer
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

In many of our lessons, we often use errors as teachable moments. Because of
this all R lessons will still render a website even if there are errors in the
examples, but this is a double-edged sword when unexpected errors happen. If you
want to prevent unexpected errors from building a lesson, you can 
[add `fail_on_error: true` to your `config.yaml` file](https://carpentries.github.io/sandpaper/reference/set_config.html#optional-keypairs-known-by-sandpaper)
and any chunks without an `error = TRUE` option will cause the build to fail if
there is an error.


