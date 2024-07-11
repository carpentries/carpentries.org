---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Hello Again"
title: "The Dovetail #6: Updates from The Carpentries Workbench"
date: 2022-08-24
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the sixth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

---

A lot has happened since the last time I provided an update (2022-07-20), just
not that much on The Workbench side of things. I attended and [presented at the RStudio conference 2022](https://zkamvar.netlify.app/talk/carpentries-rstudio-2022/),
took a short "staycation" to decompress (with a broken aircon, no less!),
attended and presented at CarpentryCon 2022, and sat on hiring committees for
our new Director of Technology. During this time, I was able to tackle some
superficial aspects of the Workbench itself. 

In this issue of The Dovetail, I wanted to reiterate the purpose of the Beta
Phase of The Workbench (which is still on hold) because it bears repeating. We
are going to be transitioning all of our lessons to use The Carpentries
Workbench starting in 2023, and the Beta Phase is here to prepare the community
for this day by doing the following:

1. Creating awareness about The Workbench and [how Workbench lessons differ from _styles_ lessons](https://carpentries.github.io/workbench/transition-guide.html).
2. Providing a risk-free sandbox for Maintainers and Instructors to work with
   The Workbench version of lessons before full transition.

If we have succeeded in the above two points, we know that we can proceed with the transition
of our lessons in 2023. However, The Workbench Beta Phase is designed to do
more than simply make the community aware of the changes; we want to make 
sure The Workbench is _thriving_ in the hands of the community. That is, we want
to: 

3. Ensure that the tool actually meets the needs and wants of the community. 
4. Create champions of, and inspire future contributors to The Workbench.

When I piloted the [Alpha Test of The Workbench]({{ site.url
}}/blog/2021/07/infrastructure-testing), my goal was to make sure that
it could be installed and work as expected for members of our community. The
move into Beta testing means that I am confident that The Workbench is indeed
stable enough to host our lessons (i.e. [the official documentation for The
Workbench](https://carpentries.github.io/sandpaper-docs/) has been continuously
hosted for the last year and a half, since 2021-02-09), and I am ready for
early adopters to try it out and really tell me how they _feel_ about The
Workbench.

This can only be really acheived with directed and specific feedback, which is
why I've given the [Beta Phase a fairly rigid structure in three stages]({{ site.url }}/blog/2022/05/workbench-beta/#beta-logistics).
During each stage, I will be asking Maintainers and Instructors to
try out different, specific, tasks and give feedback in GitHub Issues on 
[The Workbench repository](https://github.com/carpentries/workbench).
For an extra level of detail, I am hoping that I can find
some Maintainers or Instructors to provide [Friction Logs](https://github.com/carpentries/workbench/discussions/2),
which will give me a step-by-step view into a specific process so that the
exact causes of friction can be identified and smoothed out.

I really want to thank all of the current Beta Phase testers because you all
have been so patient with me as we plan out this next big step for The
Carpentries lesson infrastructure.

## Announcements

### Workbench Beta Phase Still On Hold

Just in case you did not see [The Dovetail issue number 5]({{ site.url }}/blog/2022/07/dovetail-005), the Beta phase has been put on hold so that the team could focus on time-sensitive events such as CarpentryCon and hiring for two positions. 

### Upcoming Workbench Events

#### RSECon2022 (September 2022)

Toby Hodges and I will be leading a short workshop at 
[The Conference for Research Software Engineering](https://rsecon2022.society-rse.org/) 
entitled "Collaborative Lesson Development with The
Carpentries Workbench" where we will go over the principles of lesson
development and how to use The Workbench to employ those principles. 


## Updates to The Carpentries Workbench

Since 2022-07-20, 

 - [{sandpaper} version 0.9.0 -> 0.9.3](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-093)
   - Minor maintenance fixes
   - Documentation of [configuration keys for {sandpaper}](https://carpentries.github.io/sandpaper/reference/set_config.html#default-keypairs-known-by-sandpaper).
   - Anchor links have been added to headers and callouts.
     ![Screenshot of a zoomed-in lesson website with a heading that says "Introduction". The mouse hovers next to it, revealing a chain link symbol.]({{ site.urlimg }}/blog/2022/08/dovetail-006-anchor-link.png)
 - [{varnish} version 0.2.2 -> 0.2.4](https://carpentries.github.io/varnish/news/index.html#varnish-024)
   - Heading elements are now more uniform, fixing a bug in the original design. 
   - Sidebar navigation now says "Episodes" instead of "Expand" when collapsed. 
   - The hamburger navigation menu on mobile views has a border around it to make it more obviously a button. 
 - [{pegboard} 0.3.0 -> 0.3.1](https://carpentries.github.io/pegboard/news/index.html#pegboard-031)
   - minor update for an internal function to prepare for the CRAN release of [{tinkr} 0.1.0](https://docs.ropensci.org/tinkr).

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

During the beta phase, development on The Workbench can move rapidly. While you
should be able to build your lesson successfully with any version of The
Workbench, it's a good idea to stay abreast of the packages. To keep up to date
you can run the following code in R:

```r
# Enable repository from carpentries
options(repos = c(
  ropensci = 'https://carpentries.r-universe.dev',
  CRAN = 'https://cloud.r-project.org'))
# Download and install sandpaper in R
install.packages(c('tinkr', 'pegboard', 'sandpaper', 'varnish'))
```
