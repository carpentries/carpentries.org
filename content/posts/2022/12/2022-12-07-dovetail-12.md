---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "The beta stage is extending deadlines"
title: "The Dovetail #12: Updates from The Carpentries Workbench"
date: 2022-12-07
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the twelfth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail) (our new lesson infrastructure).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, or if you have questions, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

---

## IT'S GONNA BE MAY

In our [previous blog post]({{ site.url }}/blog/2022/11/dovetail-11/), we
outlined the goals of the beta phase, acknowledged the very real situation of
limited volunteer time, and announced that we will convert all of our lessons in
mid-April 2023. Since it was published, personal considerations have required
me to reconsider the timeline and extend it. Thus, **we will convert all of our
lessons to use The Carpentries Workbench in May 2023.** Moreover, all of the
[lessons in the beta
phase](https://carpentries.github.io/workbench/beta-phase.html) will undergo
their transitions to the [beta stage](https://carpentries.github.io/workbench/beta-phase.html#beta)
_synchronously_ in February 2023. In April 2023, these lessons will 
[finalise their conversion](https://carpentries.github.io/workbench/beta-phase.html#pre-release)
and the default website will use The Workbench. 

## Why we are extending the deadline

Ultimately, we are doing this because it is better to do something right than
to do something quickly. The first shift of the beta phase placed it right in 
the middle of a time of year when members of the community may not be readily available.
This impacted the time for Maintainers to explore the lessons and it initial
design of the beta phase impacted the time and resources for organisation. This
next shift in the beta phase will mean the maintainers will have more time to
explore and also talk with each other about the experiences they are having with
The Workbench. It is my hope that, through this process, champions of The
Workbench will arise to provide feedback and fuel for its improvement.

### Time to explore the new lesson format

The transition to use The Workbench will make the lives of Instructors,
Maintainers, contributors, and Core Team staff easier when it comes to 
teaching and maintaining lessons. While Instructors will see a new format to the
lesson webpages, the Maintainers will see the repositories undergo a massive change.
Thus, the first part of the beta phase is a way for the Maintainers to get a
better sense of how the lesson repository differs in its new format without the
risk of irreversibly modifying a lesson.

### Efficiency for time and resources

When I [announced the beta phase]({{ site.url }}/blog/2022/05/workbench-beta/),
I had intended for it to start in the middle of July and run
through the end of October, giving us time to transition all of the
lessons by December. The lessons were staggered on a weekly schedule to account
for the time it would take for me to provide an [automated transition script](https://github.com/carpentries/lesson-transition#readme)
for each lesson in the beta phase. While I had taken into account [Hofstadter's law](https://en.wikipedia.org/wiki/Hofstadter%27s_law)
in planning the beta phase, situations beyond my control appeared and I had to
delay the beta phase until October. 

What I had not taken into account was the fact that I would be vastly increasing
the amount of communication work required for such a project. If every lesson
required communications before, at the beginning of, and after each stage of the
beta phase, that means that I had 49 communications to send out over
the beta phase period. 

During this last reorganisation of the beta phase schedule, all lessons will
enter the beta phase stages at the same time. This means all communications
will be synchronous so core team time can be dedicated to maintenance and
addressing Maintainer and Instructor questions. 

### Lessons Currently In the Beta Phase

The table below shows the status of lessons that are currently in the beta phase:

| Lesson                                                   | Stage[^1] |  Workbench URL                                               | Next Transition Date |
| -------------------------------------------------------- | --------- | ------------------------------------------------------------ | -------------------- |
| Data Analysis and Visualisation in R for Ecologists      | pre-beta  | <https://preview.carpentries.org/R-ecology-lesson>           | 2023-02-06           |
| R for Social Scientists                                  | pre-beta  | <https://preview.carpentries.org/r-socialsci>                | 2023-02-06           |
| Introduction to Geospatial Raster and Vector Data with R | pre-beta  | <https://preview.carpentries.org/r-raster-vector-geospatial> | 2023-02-06           |
| Instructor Training                                      | pre-beta  | <https://preview.carpentries.org/instructor-training>        | 2023-02-06           |
| Library Carpentry: The UNIX Shell                        |    -      |  https://preview.carpentries.org/lc-shell                    | 2023-12-12           |
| Análisis y visualización de datos usando Python          |    -      |  https://preview.carpentries.org/python-ecology-lesson-es    | 2023-12-12           |

[^1]: The Workbench Beta Phase is divided into three distinct stages, read more at <https://carpentries.github.io/workbench/beta-phase.html>.

## Updates to The Carpentries Workbench

Since 2022-11-16, 

 - [{sandpaper} version 0.10.7 -> 0.11.2](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0112)
   - The progress bar for episodes now reflects the fraction of time progressed
     according to the episode timings as opposed to fraction of episode pages
     visited. Thanks to an anonymous commenter to our workbench feedback form
     for this suggestion.
   - Syllabus timings are now formatted as `00h 00m` to make it more clear that
     they reflect hours and minutes and not necessarily timestamps. Thanks to
     Ross James Parker and Toby Hodges for the suggestion.
   - Internal code and documentation has been updated
 - [{pegboard} 0.3.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-032)
   - no updates :)
 - [{varnish} 0.2.9 -> 0.2.10](https://carpentries.github.io/varnish/news/index.html#varnish-0210)
   - bullet points in callouts are now better aligned with the text (thanks to
     Sarah Stevens for finding this!)

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

All lessons are set to rebuild every Tuesday at 00:00 UTC using the most recent
versions of the Workbench packages. If there is an update to a Workbench
component or an error in one of the builds, as a maintainer, you can run a new
build and your lesson will be rebuilt with the latest versions of The Workbench.

Here are the steps:

Step 1: go to `https://github.com/(ORG)/(REPO)/actions` and click on the `01 Build and Deploy` action in the sidebar

<figure style="text-align: center;">
<p>
<img alt="menu bar showing six items: code, issues, pull requests, discussions, actions (highlighted), and projects" src="{{ site.urlimg }}/blog/2022/12/dovetail-actions-tab.png" style="border: solid 1px gray; padding: 10px;">
<img alt="menu with the title 'actions' showing six workflows, the first three are numbered, followed by workflows prefixed by 'Bot'. The first workflow, '01 Build and Deploy Site' is highlighted." src="{{ site.urlimg }}/blog/2022/12/dovetail-actions-list.png" style="border: solid 1px gray; padding: 10px;">
</p>
<figurecaption>
<p> The actions menu and a subset of actions to run. Note: only the numbered actions are available to run by the maintainer.</p>
</figurecaption>
</figure>

Step 2: fill in the information and click "Run Workflow"


<figure style="text-align: center;">
<p>
<img alt="List of scheduled deploys with form overlayed that says 'use workflow from: main', 'Who triggered this build?: @zkamvar' and an unchecked box that says 'Reset cached markdown files'" src="{{ site.urlimg }}/blog/2022/12/dovetail-actions-menu.png" style="border: solid 1px gray; padding: 10px;">
</p>
</figure>
