---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Minor Delays"
title: "The Dovetail #11: Updates from The Carpentries Workbench"
date: 2022-11-16
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the eleventh post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

---

## Beta Phase Updates

Since we last met, a few bumps in the road have appeared. They are nothing 
insurmountable, but dates have been shifted a bit. Nevertheless, we will move on
with the beta phase as best we can until **April 2023 when we will convert our
entire infrastructure to use The Carpentries Workbench**.

In short: no lessons are entering [the second stage of the beta phase](https://carpentries.github.io/workbench/beta-phase.html#beta) yet. 

### Goal of The Beta Phase

In our [alpha phase testing]({{ site.url }}/blog/2021/07/infrastructure-testing/)
of The Workbench, we wanted to do a basic test to make sure that folks with
varying levels of experience with The Carpentries, R, and our lesson
infrastructure could perform a fixed set of tasks that could confirm to us that
the infrastructure was usable. What this test did _not_ give us was an
understanding of how it would perform in a dynamic environment of a lesson. 

The goal of the beta phase was to test the new infrastructure with real live
lessons and people who would be directly affected by the change of the lesson
infrastructure; that is, lesson Maintainers, Instructors, and Learners. 

In order for a lesson to enter the beta phase, all of the Maintainers had to
consent to the process. 

Because the entire structure of the lessons would change, it was important
that I have evidence that Maintainers are able to perform the following tasks
for their lessons:

1. clone the lesson to their local machine and preview it
2. make a change to the lesson and confirm that it shows up on the website
3. review and merge a pull request

Ideally, these actions would be completed in [the pre-beta stage](https://carpentries.github.io/workbench/beta-phase.html#pre-beta) 
of the beta phase so that Maintainers can have a handle on what working with a 
Workbench lesson feels like before there is no turning back.

### It Is Okay To Ask for More Time

The Carpentries is a community of volunteers and time is a precious commodity.
If a Maintainer has more urgent obligations, it is perfectly fine and
understandable for them to take a step back from their maintenance duties
without notice.

The three criteria I listed above are important for working in the pre-beta stage
of the beta phase, but it is not required. The only requirement to move out of
the pre-beta stage is that all of the open pull requests are resolved (merged 
or closed).

It is because of this requirement that the [Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson)
lesson Maintainers decided to remove their lesson from the beta phase. They were
undergoing a substantial rewrite of the lesson and would not be able to review and
merge these changes in enough time.

I had also checked in with the lesson Maintainers from the other lessons that
had entered the beta phase and some were responsive, some non-responsive. In
light of the responses, the following transitions have been put on hold or delayed:


 - [Data Analysis and Visualization in R for Ecologists](https://github.com/datacarpentry/R-ecology-lesson/) (pre-beta; on hold)
 - [R for Social Scientists](https://github.com/datacarpentry/r-socialsci/) (pre-beta; delayed 2 weeks)
 - [Introduction to Geospatial Raster and Vector Data with R](https://github.com/datacarpentry/r-raster-vector-geospatial/) (pre-beta; on track)
 - [Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson/) (cancelled)
 - [Library Carpentry: The UNIX Shell](https://github.com/LibraryCarpentry/lc-shell/) (on hold)
 - [Instructor Training](https://github.com/carpentries/instructor-training/) (on track)
 - [Análisis y visualización de datos usando Python](https://github.com/datacarpentry/pthon-ecology-lesson-es/) (on track)


### Lessons Currently In the Beta Phase

[R for Social Scientists](https://datacarpentry.org/r-socialsci) and 
[Introduction to Geospatial Raster and Vector Data with R](https://datacarpentry.org/r-raster-vector-geospatial) 
have both entered into the Workbench Beta Phase. The table below shows the
status of lessons that are currently in the beta phase:

| Lesson                                                   | Stage[^1] |  Workbench URL                                               | Next Transition Date |
| -------------------------------------------------------- | --------- | ------------------------------------------------------------ | -------------------- |
| Data Analysis and Visualisation in R for Ecologists      | pre-beta  | <https://preview.carpentries.org/R-ecology-lesson>           | TBA                  |
| R for Social Scientists                                  | pre-beta  | <https://preview.carpentries.org/r-socialsci>                | 2022-12-06           |
| Introduction to Geospatial Raster and Vector Data with R | pre-beta  | <https://preview.carpentries.org/r-raster-vector-geospatial> | 2022-11-28           |

[^1]: The Workbench Beta Phase is divided into three distinct stages, read more at <https://carpentries.github.io/workbench/beta-phase.html>.

## Updates to The Carpentries Workbench

Since 2022-11-02, 

 - [{sandpaper} version 0.10.6 -> 0.10.7](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0107)
   - Workflows have been updated to no longer throw warnings of deprecated GitHub commands
   - Automated pull requests will now go to a single branch for each type of pull request, updating as needed.
     This prevents the situation where there are multiple pull requests open from [@carpentries-bot](https://github.com/carpentries-bot), 
     with the last one superseding the previous ones. 
 - [{pegboard} 0.3.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-032)
   - no updates :)
 - [{varnish} 0.2.8 -> 0.2.9](https://carpentries.github.io/varnish/news/index.html#varnish-028)
   - matomo analytics have been temporarily disabled.

To update your local Workbench installation, open R and use the following code:

```r
# Enable repository from carpentries
options(repos = c(
  ropensci = 'https://carpentries.r-universe.dev',
  CRAN = 'https://cloud.r-project.org'))
# Download and install sandpaper in R
install.packages(c('tinkr', 'pegboard', 'sandpaper', 'varnish'))
```

## Tips and Tricks for Using The Workbench

Make sure you stay hydrated and take time for self-reflection. 
