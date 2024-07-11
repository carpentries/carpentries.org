---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Ode to Maintainers"
title: "The Dovetail #13: Updates from The Carpentries Workbench"
date: 2022-12-21
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the thirteenth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail) (our new lesson infrastructure).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, or if you have questions, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

---

## Last Dovetail of the Year

This installment of The Dovetail will be the last one of 2022. In 2023, we will
resume posting The Dovetail, but we will slow the pace down to once a month, on
the third Tuesday of the month. For this last installment, I wanted to take the
time to express my gratitude to a very important part of our community.

### Thank You Lesson Maintainers

At its core, The Carpentries is a community of volunteers. These volunteers come
together to bring data and coding skills to researchers around the globe, and 
they do this through a core set of lessons in our three main curricula: Data
Carpentry, Library Carpentry, and Software Carpentry. One of the special things
about our lessons is that they are constantly updated with community feedback to
highlight areas that work well and bring support to areas that need reworking.

All of our official lessons are maintained by our [Lesson Maintainers]({{ site.url }}/maintainers).
This is a dedicated group of volunteers who have domain expertise and
understand the nuances of The Carpentries model of instruction and lesson
design. They, in collaboration with the Curriculum Advisory Committees, are
responsible for ensuring that our lessons remain up-to-date and relevant to the
ever shifting landscape of software while still teaching fundamental skills for
beginners.

The job of a Maintainer is not always an easy one. A lesson is a complex
production with many stakeholders, goals, and outcomes wrapped in a time-limited
package that is open and available to all. When contributions come in, the
Maintainers are tasked with assessing the contribution and determining if it
belongs in the lesson. Some contributions (i.e. typos) are straightforward to
accept, but other contributions take much more time to evaluate, discuss, and
come to a decison.

One key element about our Maintainer community is that they are often the folks
who are interacting with people who may be contributing to GitHub for the very
first time. It can often be very intimidating to submit an issue or pull request
and our Maintainers are the humanity behind the repository. So this is for all
the Maintainers who took time to say "Thank you" while merging a pull request
from a beginner, for all those who had to ask their fellow Maintainers for help
with a particularly tricky issue, for those who have crafted a gentle way to say
'no' to a contribution that would have increased the timing of an episode, and
for all of our Maintainers for being a compassionate part of our community that
embodies and champions our core values.

## Lessons Currently In the Beta Phase

The table below shows the status of lessons that are currently in the beta phase. 
All of these lessons are currently in the [pre-beta stage](https://carpentries.github.io/workbench/beta-phase.html#pre-beta) (two repositories, two lesson websites) 
and will transition to the [beta stage](https://carpentries.github.io/workbench/beta-phase.html#beta) (one repository, two lesson websites) on 2022-02-06.

| Lesson                                                   | Workbench URL                                                |
| -------------------------------------------------------- | ------------------------------------------------------------ |
| Data Analysis and Visualisation in R for Ecologists      | <https://preview.carpentries.org/R-ecology-lesson>           |
| R for Social Scientists                                  | <https://preview.carpentries.org/r-socialsci>                |
| Introduction to Geospatial Raster and Vector Data with R | <https://preview.carpentries.org/r-raster-vector-geospatial> |
| Instructor Training                                      | <https://preview.carpentries.org/instructor-training>        |
| Library Carpentry: The UNIX Shell                        | <https://preview.carpentries.org/lc-shell>                   |
| Análisis y visualización de datos usando Python          | <https://preview.carpentries.org/python-ecology-lesson-es>   |

[^1]: The Workbench Beta Phase is divided into three distinct stages, read more at <https://carpentries.github.io/workbench/beta-phase.html>.

## Updates to The Carpentries Workbench

Since 2022-12-06, 

 - [{sandpaper} version 0.11.2 -> 0.11.3](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0113)
   - Workflows have been updated to avoid [false alarm pull request comments](https://github.com/carpentries/lesson-development-training/pull/165#issuecomment-1337182275)
     triggered by commits pushed to a PR in rapid succession. With this update,
     running workflows will give precedence to new workflows created with new
     pushes.
 - [{pegboard} 0.3.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-032)
   - no updates :)
 - [{varnish} 0.2.10 -> 0.2.11](https://carpentries.github.io/varnish/news/index.html#varnish-0211)
   - Printing of lesson pages is better formatted for teaching by expanding
     solutions and instructor notes, adding boxes around callouts, and removing
     extraneous navigational content.

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

It's okay to rest. Happy New Year, y'all.
