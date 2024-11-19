---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Working through chopportunities"
title: "The Dovetail #3: Updates from The Carpentries Workbench"
date: 2022-06-22
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the third post in a series that we are calling "The Dovetail."
In this series, we aim to keep members of The Carpentries community abreast of
the current news for [The Carpentries Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

## Updates to The Carpentries Workbench

Since 2022-06-08, 

 - [{sandpaper} version 0.5.8 -> 0.6.0](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-060)
   - `create_episode()` will now accept titles with spaces and UTF-8 characters. 
      A slugified file name will be created from the title. 
      Now you can create a new episode like so:
      `sandpaper::create_episode("안녕 고양이 😹 Hello Kitty!")` and the 
      corresponding file name will be: `02-안녕-고양이-😹-hello-kitty.Rmd`
   - `create_episode()` now has the variants `create_episode_rmd()` and 
     `create_episode_md()`, for lesson developers who want to create episodes
     of a specific file type.
   - `create_lesson()` gains the `rmd = TRUE` argument, which allows lesson 
     developers to opt out of creating an R Markdown-based episode if they want. 
 - [{varnish} version 0.1.14 -> 0.2.0](https://carpentries.github.io/varnish/news/index.html#varnish-020)
   - The search field has been disabled to avoid confusion (it is a future endeavour)
   - The heading above the sidebar has been renamed to `EPISODES` to avoid confusion
   - The sidebar will stay collapsed across page refreshes
 - [{pegboard} (no updates)](https://carpentries.github.io/pegboard/news/index.html#pegboard-030)
 - Both the [markdown template](https://github.com/carpentries/workbench-template-md) and [R Markdown template](https://github.com/carpentries/workbench-template-rmd)
   now default to creating incubator lessons, as these are more common than lessons that are purely carpentries.

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

Zhian (aka Workbench DevOps Lead; aka Workbench Q&A Lead; aka Workbench Beta
Phase Lead; aka Workbench Communications Lead) was on a well-deserved holiday
last week, so the status since [our last update to the Workbench Beta
Phase](https://carpentries.org/blog/2022/06/dovetail-002/#updates-to-the-carpentries-workbench)
has not changed much. 

### List of Lessons to enter Workbench Beta in 2022

No lessons have yet entered Workbench Beta, but we have a list of lessons that
are in the queue:

#### Official Lessons

 - [datacarpentry/R-ecology-lesson---Data Analysis and Visualization in R for Ecologists](https://github.com/datacarpentry/R-ecology-lesson/discussions/799) (✅ approved by maintainers)
 - [datacarpentry/r-socialsci---R for Social Scientists](https://github.com/datacarpentry/r-socialsci) (✅ approved by maintainer)
 - [datacarpentry/r-raster-vector-geospatial---Introduction to Geospatial Raster and Vector Data with R](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/369) (⏳ awaiting responses)
 - [datacarpentry/OpenRefine-ecology-lesson---Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson) (✅ approved by maintainer)
 - [librarycarpentry/lc-shell---Library Carpentry: The UNIX Shell](https://github.com/librarycarpentry/lc-shell) (⏳ awaiting responses)
 - [carpentries/instructor-training---Instructor Training](https://github.com/carpentries/instructor-training) (⏳ awaiting responses)

##### Tentative schedule for official lessons

Here are the tentative dates for lessons to enter pre-beta starting in the
middle July. Please note that these dates are strictly _tentative_ and are
subject to change due to several factors including obligations that arise due
to CarpentryCon.

| Lesson                                                   | Date Entering Pre-Beta |
|----------------------------------------------------------| ---------------------- |
| Data Analysis and Visualization in R for Ecologists      | 2022-07-12 |
| R for Social Scientists                                  | 2022-07-19 |
| Introduction to Geospatial Raster and Vector Data with R | 2022-07-26 |
| Data Cleaning with OpenRefine for Ecologists             | 2022-08-02 |
| Library Carpentry: The UNIX Shell                        | 2022-08-16 |
| Instructor Training                                      | 2022-08-23 |

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

### New Participants

From our [original call for participants in the workbench beta phase]({{
site.url }}/blog/2022/05/workbench-beta/), we have gotten three new responses,
for a total of twenty community members officially participating in the beta
phase:

 - **Eirini Zormpa, Maintainer**
 - **James Sadler, Maintainer**
 - **[Robin](https://github.com/longr/), Instructor**
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

## Updates from Community About Working in Workbench Beta

The developers of the [Collaborative Lesson Development Training
Curriculum](https://carpentries.github.io/lesson-development-training/) ran
their alpha pilot recently and Toby Hodges had this to say about their experience:

> [The Workbench](https://carpentries.github.io/workbench) was really a breeze
> to work with in [the [collaborative lesson development]
> training](https://carpentries.github.io/lesson-development-training/) pilot
> last week. The participants seemed to get the hang of it very quickly, and it
> was so much easier to keep them focussed on the relevant parts while giving
> the training than it would have been with
> [styles](https://github.com/carpentries/styles). We heard a lot of positive
> feedback about how the lesson sites look, and the ease with which the various
> components fit together. 

Additionally, I have created a **Testimonials category** for The Workbench
discussion forum so that people can share their insights. If you have used the
workbench in _any_ way shape or form, I strongly encourage you to share your
experience and get others excited: <https://github.com/carpentries/workbench/discussions/categories/testimonials>

## Tips and Tricks for Using The Workbench

[Callout blocks](https://carpentries.github.io/sandpaper-docs/episodes.html#callout-blocks) 
are always in the form of fenced divs that start with _at least_ three
colons followed by a class tag and end with a line that is comprised solely of
_at least_ three colons.


```markdown
::: callout

### This is

A callout block

:::::::::::
```

If you want to find out what types of callout blocks are avialable, you can
check out the [Workbench Component Guide](https://carpentries.github.io/sandpaper-docs/component-guide.html),
which displays the output of components that can be created with fenced divs.

