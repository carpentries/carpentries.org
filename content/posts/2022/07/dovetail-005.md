---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Workbench Beta on Hold"
title: "The Dovetail #5: Updates from The Carpentries Workbench"
date: 2022-07-20
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the fifth post in a series that we are calling "The Dovetail."
In this series, we aim to keep members of The Carpentries community abreast of
the current news for [The Carpentries Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

## Announcements

### Workbench Beta Phase On Hold

**The Workbench Beta phase is [on Hold until after CarpentryCon](https://github.com/carpentries/workbench/discussions/22)**, 
and it is likely that it will be on hold until mid-September. Over the last few
weeks, [like an unexpected late spring ice storm](https://www.weather.gov/gjt/Jan09_IceStorm),
situations unrelated to development of The Workbench both personal and
professional ([such as the departure of a good friend and colleague]({{ site.url }}/blog/2022/07/thank-you-francois/))
have arisen, which forced me to stop pedaling and gently squeeze the brakes on
this project so that the Dovetail does not turn into [a fishtail](https://en.wikipedia.org/wiki/Fishtailing).

**What does this mean for the folks who have already signed up for the beta phase?**
It means that the schedule is delayed by a couple of months. This will give me 
enough time provide better documentation and coordination regarding The Beta
Phase. In the end, the participants will end up with a better experience in
working with their lessons than if I had rushed through with the Beta on the
initial tentative schedule.

This is not a post that I am particularly excited about writing, especially
since this project represents the vast majority of my work as Carpentries staff.
That being said, I am proud to write this post because it embodies two of our 
[core values](https://carpentries.org/values): always learning, always acting
openly, and championing people first. By setting aside the Beta Phase for a
moment, I am able to focus more energy on preparing materials for the upcoming
skillups I have for CarpentryCon. Moreover, this time will give me more
opportunities to bolster The Workbench documentation so that the onramps are
that much smoother. Ultimately, I am proud to write this post because I want to
live in a world where it is okay to take a step back and move slowly when
conditions change suddenly. While others like to release and iterate or move
fast and break things, I prefer to slow down and make sure others can still see
the light from my torch.

### Upcoming Workbench Events

#### RStudio Conference (July 2022)

I will be giving a talk about The Workbench at the RStudio Conference entitled
["Building Accessible Lessons with R and Friends" on Thursday, July 28, 2022
at 13:50 EST](https://rstudioconf2022.sched.com/event/866f939b8e168ae0c191421e7a58bf86?). 
The talk will be recorded and will be available for all after the
conference concludes. In the talk I will highlight how we used our Core Values
to design The Carpentries Workbench.


#### CarpentryCon (August 2022)

CarpentryCon is coming up at the beginning of August (so you should [register to attend (its free!)](https://2022.carpentrycon.org/)) 
and there will be several opportunities to learn about The Workbench at the
Skillup entitled: "Building Lessons with The Carpentries Workbench" lead by
Toby Hodges and myself. Check out the times:

 - 10 August, 2022 09:30-11:30 UTC [(add to your calendar)](https://www.google.com/calendar/event?eid=N2xtMG8ydXUwOGM5amptY3FqbjBsMWFldTkgY190bXRya2YzMjhnanRjczF1MDVtaGZibjdxY0Bn)
 - 10 August, 2022 22:00-00:00 UTC [(add to your calendar)](https://www.google.com/calendar/event?eid=NGpmZnVmamJ1MGFqMTRzdjJsYTZsODA3YmggY190bXRya2YzMjhnanRjczF1MDVtaGZibjdxY0Bn)
 - 12 August, 2022 14:00-16:00 UTC [(add to your calendar)](https://www.google.com/calendar/event?eid=N2lvOXM4c2F2MmJpOG4yODlmZ2hlNDliYmYgY190bXRya2YzMjhnanRjczF1MDVtaGZibjdxY0Bn)

#### RSECon2022 (September 2022)

Toby Hodges and I will be leading a short workshop at 
[The Conference for Research Software Engineering](https://rsecon2022.society-rse.org/) 
entitled "Collaborative Lesson Development with The
Carpentries Workbench" where we will go over the principles of lesson
development and how to use The Workbench to employ those principles. 


## Updates to The Carpentries Workbench

Since 2022-07-06, 

 - [{sandpaper} version 0.7.1 -> 0.9.0](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-090)
   - Automated Pull Request comments are now more informative and have been set
     up to provide an automated check on unknown PRs so that the maintainer knows
     if they can safely build the pull request previews. 
   - `set_config()` gains the option `create` to create new variables in 
     `config.yaml` if they do not exist
 - [{varnish} version 0.2.0 -> 0.2.2](https://carpentries.github.io/varnish/news/index.html#varnish-022)
   - A bug in tablet/mobile view where extra pages were not listed in the menu was fixed.
   - The formatting of list elements in solutions and instructor notes have been fixed.
 - [{pegboard} (no updates)](https://carpentries.github.io/pegboard/news/index.html#pegboard-030)

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

Stay Tuned for CarpentryCon!
