---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "R for Ecologists has entered the pre-beta stage"
title: "The Dovetail #9: Updates from The Carpentries Workbench"
date: 2022-10-19
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

## Beta Phase Updates

The beta phase is up and running with the first lesson: "Data Analysis and
Visualisation in R for Ecologists". The live version is at
<https://datacarpentry.org/R-ecology-lesson>, while The Workbench version is at
<https://preview.carpentries.org/R-ecology-lesson>. Note that The Workbench
version of the lesson is a snapshot from 2022-10-17, which allows the
Maintainers of the lesson to practise working with the new infrastructure before
it becomes the default. On 2022-11-14, the underlying lesson repository will
be converted to using the Workbench. During this time, the default URL will serve
a snapshot of the lesson, and the live lesson will be served at the preview URL.
Note that any pull requests that come into the lesson during that time should
not come from forks created before 2022-11-14. 

In the next two weeks, two further lessons will enter the beta phase:

 - [R for Social Scientists](https://datacarpentry.org/r-socialsci)
 - [R for Raster and Vector Data](https://datacarpentry.org/r-raster-vector-geospatial/)

For Instructors, here is a video showing what you can expect to see when you go
to teach a lesson that is entering the beta phase:

<iframe width="560" height="315" src="https://www.youtube.com/embed/B3J9eJ6TUwY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Updates to The Carpentries Workbench

Since 2022-10-05, 

 - [{sandpaper} version 0.10.1 -> 0.10.4](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0104)
   - A workaround for a [bug in {renv} 0.16.0](https://github.com/rstudio/renv/issues/1088) has been added to prevent extra files from being committed to the renv/ folder in R lessons.
   - Weekly workflow file pull requests no longer result in pull requests with only sandpaper-version.txt changed.
 - [{pegboard} 0.3.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-032)
   - no updates :)
 - [{varnish} 0.2.4 -> 0.2.6](https://carpentries.github.io/varnish/news/index.html#varnish-026)
   - Lessons that have `workbench-beta`, `old-url`, and `pre-beta-date` tags
     will now display a modified alert banner that will give information about
     when the lesson entered the beta phase and will link back to the default
     lesson URL.

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

If you are developing a lesson and you want to move a single episode to a 
different place in the schedule, you can use the [`move_episode()` function](https://carpentries.github.io/sandpaper/reference/move_episode.html):

For example, if you have the following episodes and wanted to move library before
data:

 - introduction.md
 - data.md
 - software.md
 - library.md
 - outro.md

You could use the move command to interactively select where you want to insert
the episode:

```r
library("sandpaper")
move_episode("library.md", write = TRUE)
```

You would see a menu that prompts you to move the episode: 

```output
ℹ Select a number to insert your episode
(if an episode already occupies that position, it will be shifted down)

1. introduction.md
2. data.md
3. software.md
4. library.md
5. outro.md

Choice: 2
```
