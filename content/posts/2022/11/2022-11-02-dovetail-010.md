---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "R for Social Scientists and R for Geospatial Data have entered the Beta Phase"
title: "The Dovetail #10: Updates from The Carpentries Workbench"
date: 2022-11-02
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the tenth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM' style=''>tell us about your experience</a>.</b></span> 

---

## Beta Phase Updates

### Lessons Currently In the Beta Phase

[R for Social Scientists](https://datacarpentry.org/r-socialsci) and 
[Introduction to Geospatial Raster and Vector Data with R](https://datacarpentry.org/r-raster-vector-geospatial) 
have both entered into the Workbench Beta Phase. The table below shows the
status of lessons that are currently in the Beta Phase:

| Lesson                                                   | Stage[^1] |  Workbench URL                                               | Next Transition Date |
| -------------------------------------------------------- | --------- | ------------------------------------------------------------ | -------------------- |
| Data Analysis and Visualisation in R for Ecologists      | pre-beta  | <https://preview.carpentries.org/R-ecology-lesson>           | 2022-11-14           |
| R for Social Scientists                                  | pre-beta  | <https://preview.carpentries.org/r-socialsci>                | 2022-11-28           |
| Introduction to Geospatial Raster and Vector Data with R | pre-beta  | <https://preview.carpentries.org/r-raster-vector-geospatial> | 2022-11-28           |

[^1]: The Workbench Beta Phase is divided into three distinct stages, read more at <https://carpentries.github.io/workbench/beta-phase.html>.

When you visit these pages, if you want to go back to the original lesson, you 
can click on the workbench beta alert icon at the top of the page:

<figure style='text-align: center;'>
<img alt='screencapture of pre-beta alert box on a Workbench site with a yellow caution icon followed by the text &quot;Workbench Beta | Give Feedback | Learn More&quot;. The &quot;give feedback&quot; and &quot;learn more&quot; are links in bold.' src='{{ site.urlimg }}/blog/2022/11/dovetail-010-pre-beta-alert.png' style='border: solid 1px gray; padding: 10px;' />
<figcaption>
Alert banner displayed for lessons in Workbench pre-beta stage
</figcaption>
</figure>

For Instructors, here is a video showing what you can expect to see when you go
to teach a lesson that is entering the beta phase:

<iframe width="560" height="315" src="https://www.youtube.com/embed/B3J9eJ6TUwY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### Upcoming Lessons

In the next two weeks, we will see the following lessons enter the beta phase:

 - [Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson) (2022-11-07)
 - [Library Carpentry: The UNIX Shell](https://github.com/librarycarpentry/lc-shell) (2022-11-14)

### Links to edit pages

During the beta phase, there will be two parallel sites available for 12 weeks,
one that is live and will continue to recieve updates and the other that serves
as a snapshot as demonstrated in this table:

| phase    | live site               | snapshot                  | snapshot editable? | 
| -------- | ----------------------- | ------------------------- | ------------------ |
| pre-beta | `carpentries.github.io` | `preview.carpentries.org` | yes                |
|     beta | `preview.carpentries.org` | `carpentries.github.io` | no                 |

[A recent question from the Workbench GitHub Discussions](https://github.com/carpentries/workbench/discussions/30)
asks:

> If learners/trainees are presented with a "snapshot" version of a lesson,
> will clicking that button send them to the snapshot repo? If so, will there
> be any messaging (banners etc) to redirect them to the correct repo for
> making contributions?

We value all contributions and do not want the beta phase to introduce a barrier that could prevent a community member from improving a lesson.
If someone clicks on a link, makes a suggested change, and opens a pull request,
it would be demotivating to find out that the contribution was made to a
temporary or frozen version of the lesson. Thus, the [answer to this question](https://github.com/carpentries/workbench/discussions/30#discussioncomment-3955501) 
is that clicking on the "improve this page" or "edit this page" buttons will
lead contributors to a landing page that briefly explains the purpose of the
phase they entered the lesson through and provides a link to follow to make their
suggestion to the lesson.

For example, if the contributor clicks on a link from a snapshot in pre-beta
stage where it _is_ editable, but not permanent, they would find the following
page: 

<figure style="text-align: center;">
<img src="{{ site.urlimg }}/blog/2022/11/dovetail-010-edit-workbench.png" alt="screenshot of a portion of the workbench lesson episode &quot;Before we Start&quot; that shows it was Last updated on 2022-10-31 with a link that says &quot;Edit this page&quot;" style="border: solid 1px gray; padding: 10px;">
<img src="{{ site.urlimg }}/blog/2022/11/dovetail-010-pre-beta-screen.png" alt="screenshot that shows the landing page for the pre-beta stage. Text with a link at the bottom says &quot;You may continue to propose changes to the temporary snapshot of this lesson&quot;" style="max-width: 100%;">
<figcaption>When the reader clicks on the link that says "Edit this page", the will they would find 
<a src="https://carpentries.github.io/workbench/contributor/pre-beta.html?id=https://github.com/fishtree-attempt/r-socialsci/edit/main/episodes/00-intro.Rmd">the pre-beta snapshot page</a>
</figcaption>
</figure>

If a lesson is in the beta stage, where the snapshot _is not_ editable, they 
would find the following page: 

<figure style="text-align: center;">
<img src="{{ site.urlimg }}/blog/2022/11/dovetail-010-edit-styles.png" alt="screenshot of a button that says &quot;Improve this page&quot;" style="border: solid 1px gray; padding: 10px;">
<img src="{{ site.urlimg }}/blog/2022/11/dovetail-010-beta-screen.png" alt="screenshot that shows the landing page for the beta stage. Text with a link at the bottom says &quot;You may continue to propose changes to the live lesson&quot;" style="max-width: 100%;">
<figcaption>When the reader clicks on the link that says "Improve this page", the will they would find 
<a src="https://carpentries.github.io/workbench/contributor/beta.html?id=https://github.com/datacarpentry/r-socialsci/edit/main/_episodes_rmd/00-intro.Rmd">the beta snapshot page</a>
</figcaption>
</figure>


## Updates to The Carpentries Workbench

Since 2022-10-19, 

 - [{sandpaper} version 0.10.4 -> 0.10.6](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0106)
   - The `move_episode()` and `set_` family of functions will now print the command to use if the user calls the function without `write = TRUE`
 - [{pegboard} 0.3.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-032)
   - no updates :)
 - [{varnish} 0.2.6 -> 0.2.8](https://carpentries.github.io/varnish/news/index.html#varnish-028)
   - Bugs in the Workbench beta phase links have been fixed
   - Links to edit pages on GitHub are now directed to a page that first explains the purpose of the beta phase.

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
| [datacarpentry/r-socialsci---R for Social Scientists](https://github.com/datacarpentry/r-socialsci) (✅ approved by maintainer) | 2022-10-31 | 2022-11-28 | 2023-02-06 |
| [datacarpentry/r-raster-vector-geospatial---Introduction to Geospatial Raster and Vector Data with R](https://github.com/datacarpentry/r-raster-vector-geospatial/issues/369) (✅ approved by maintainers) | 2022-10-31 | 2022-11-28 | 2023-02-06  |
| [datacarpentry/OpenRefine-ecology-lesson---Data Cleaning with OpenRefine for Ecologists](https://github.com/datacarpentry/OpenRefine-ecology-lesson) (✅ approved by maintainer) | 2022-11-07 | 2022-12-05 | 2023-02-13  |
| [librarycarpentry/lc-shell---Library Carpentry: The UNIX Shell](https://github.com/librarycarpentry/lc-shell) (✅ approved by maintainers) | 2022-11-14 | 2022-12-12 | 2023-02-20  |
| [carpentries/instructor-training---Instructor Training](https://github.com/carpentries/instructor-training/issues/1396) (✅ approved by maintainers) | 2022-11-28 | 2023-01-09 | 2023-03-06  |
| [datacarpentry/python-ecology-lesson-es---Análisis y visualización de datos usando Python](https://github.com/datacarpentry/python-ecology-lesson-es) (✅ approved by maintainers) | 2022-12-05 | 2023-01-16 | 2023-03-13  |


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

**This tip is for folks who are working on lessons that use R Markdown.**

This tip will show you how to use the package cache to debug a problem in your
lesson without changing your default R package library.

Lessons that use the Workbench automatically use [the {renv}
package](https://rstudio.github.io/renv) to manage lesson dependencies without
modifying the state of your default R package library. This is different than the
styles version of the lessons where you would be forced to update the packages
in your global package library. 
In a lesson, the lockfile for this package cache lives in 
[renv/profiles/lesson-requirements/renv.lock](https://github.com/carpentries/sandpaper-docs/tree/main/renv/profiles/lesson-requirements/renv.lock).


Now imagine that there is a mysterious error in your lesson. Take for example
[PR#378](https://github.com/datacarpentry/r-raster-vector-geospatial/pull/378)
for one of the lessons that was released into pre-beta today. This error
happened because there was a change in a package that was used. This led to a
problem with some of the plotting commands where there would be an error that
looked something like this:

```
Error in FUN(X[[i]], ...): object 'HARV_RGB_Ortho.3' not found
```

There are two ways to diagnose the error: 

### Solution 1: copy files and use renv

You can create a new folder outside of your lesson and copy the `renv.lock`
file into that folder along with the data and files from the `episodes/` folder. 
When you open R inside that folder type:

```r
renv::restore()
```

Once you have that, you can run through the commands until you get to the error.

### Solution 2: use `work_with_cache()`

I wrote the [`work_with_cache()` function](https://carpentries.github.io/sandpaper/reference/work_with_cache)
in the {sandpaper} package to temporarily allow me to use the versions in the
package cache while I was working on the [transition workflow](https://github.com/carpentries/lesson-transition). It allowed me to quickly access packages to build the
lesson without having to reinstall them to my default library. 

To debug, I open the R Markdown file that was giving me trouble and set my
working directory to `site/built` where all of the intermediate Markdown output
is rendered. After that I call `work_with_cache()` placing the output in a
variable called "done".

```r
library(sandpaper)
setwd("site/built")
done <- work_with_cache() # loads the lesson-requirements profile
```

Once I do this, My prompt looks like this:

```
* (lesson-requirements) Project '/path/to/r-raster-vector-geospatial' loaded. [renv 0.16.0]
ℹ call `done()` when you are finished with the session.

[lesson]> 
```

And then I can walk through the R Markdown document until I hit the error and 
begin exploring. When I find the solution, I can fix it in the document and 
then restore my session by calling `done()`, which is a function that 
`work_with_cache()` created to finalise the session and return you to your
previous state.

```r
done() # detaches the lesson-requirements profile, allowe me to access my default library
```

