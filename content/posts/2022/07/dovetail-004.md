---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Community Discussions Coming Up!"
title: "The Dovetail #4: Updates from The Carpentries Workbench"
date: 2022-07-03
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail", "Workflows"]
---

This is the fourth post in a series that we are calling "The Dovetail."
In this series, we aim to keep members of The Carpentries community abreast of
the current news for [The Carpentries Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

## Announcements

For anyone who has questions about The Workbench, [I will be hosting two themed
community discussions](https://pad.carpentries.org/community-discussions):

 - (UTC) Friday 08 July 2022 14:00 ([find your time](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Themed+Community+Discussion:+Workbench+Listening+Session+1&iso=20220708T1400))
 - (UTC) Tuesday 12 July 2022 00:00 ([find your time](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Themed+Community+Discussion:+Workbench+Listening+Session+1&iso=20220708T1400))

## Updates to The Carpentries Workbench

Since 2022-06-08, 

 - [{sandpaper} version 0.6.0 -> 0.7.1](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-071)
   - Creating a new lesson from the R package now defaults to an Incubator lesson.
   - If you have a lesson that uses R Markdown and want unexpected errors to cause build failures,
     place `fail_on_error: true` in your lesson's `config.yaml` file.
 - [{varnish} version 0.1.14 -> 0.2.0](https://carpentries.github.io/varnish/news/index.html#varnish-020)
   - Sidebar navigation on mobile and tablet views now includes all the information
     that was included in the navigation bar for desktop mode.
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

By this time next week, [datacarpentry/R-ecology-lesson---Data Analysis and Visualization in R for Ecologists](https://github.com/datacarpentry/R-ecology-lesson/discussions/799) (✅ approved by maintainers) will enter **Workbench Pre-Beta** which means that a snapshot
of the lesson will be available at 
<https://lessons.datacarpentry.org/R-ecology-lesson> (note: there is no page here
yet). 

#### Official Lessons

 - [datacarpentry/R-ecology-lesson---Data Analysis and Visualization in R for Ecologists](https://github.com/datacarpentry/R-ecology-lesson/discussions/799) (✅ approved by maintainers)
 - [datacarpentry/r-socialsci---R for Social Scientists](https://github.com/datacarpentry/r-socialsci) (✅ approved by maintainer)
 - [datacarpentry/r-raster-vector-geospatial---Introduction to Geospatial Raster and Vector Data with R](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/369) (⏳ awaiting responses)
 - [datacarpentry/OpenRefine-ecology-lesson---Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson) (✅ approved by maintainer)
 - [librarycarpentry/lc-shell---Library Carpentry: The UNIX Shell](https://github.com/librarycarpentry/lc-shell) (⏳ awaiting responses)
 - [carpentries/instructor-training---Instructor Training](https://github.com/carpentries/instructor-training) (⏳ awaiting responses)

##### Tentative schedule for official lessons

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

## Updates from Community About Working in Workbench Beta


## Tips and Tricks for Using The Workbench

If you maintain a lesson on The Carpentries Infrastructure, you get the 
following [Automated pull requests](https://carpentries.github.io/sandpaper-docs/instructor/pull-request.html#automated-pull-requests)
that help you ensure your lesson stays up-to-date and healthy:

1. A weekly pull request that checks for updates to GitHub Workflows
2. (for R-based lessons) a monthly pull request that updates the versions of packages used in the lesson

Both of these pull requests are issued by
[@carpentries-bot](https://github.com/carpentries-bot), but if you are not a
member of a Carpentries organisation, then you will not get these pull
requests, but you can still update locally with the following {sandpaper} calls:

```r
library("sandpaper")
update_github_workflows() # update the github workflows to your version of sandpaper
update_cache() # update the package cache to use the latest versions of the packages in your lesson
```

If you have a lesson outside of The Carpentries and do not want to do this
manually, you can still get access to pull requests like this, and [the
workflow will remind you to do
this](https://github.com/zkamvar/potential-porpoise/actions/runs/2573082987)
with the following instructions: 

### Steps to Generate a New Token

1. :key: Go to https://github.com/settings/tokens/new to generate a new token with the `repo` and `workflow` scopes from your GitHub Account and give it a name that's meaningful
2. :clipboard: Copy your new token to your clipboard
3. Go To https://github.com/YOUR-ACCOUNT/YOUR-REPOSITORY/settings/secrets/actions/new
   - enter `SANDPAPER_WORKFLOW` for the 'Name'
   - :inbox_tray: paste your token for the 'Value'

After that, your lesson will have the benefits of automated pull requests that
keep you up-to-date!

