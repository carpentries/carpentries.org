---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Beta Phase to enter stage 2 in February"
title: "The Dovetail #14: Updates from The Carpentries Workbench"
date: 2023-01-17
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the fourteenth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail) (our new lesson infrastructure).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 
If you are unfamiliar with The Workbench, you can [watch a video that describes
the workbench and the beta phase in twom minutes](https://youtu.be/x7tETGpF3-4).

If you are interested in participating in discussions around The Carpentries
Workbench, or if you have questions, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

---

## Entering the Second Stage of the Beta Phase

### Beta Phase So Far

Since December, the [lessons currently in the beta phase](#lessons-currently-in-the-beta-phase) have been in the 
[first (pre-beta) stage](https://carpentries.github.io/workbench/beta-phase.html#pre-beta) of the
beta phase: **two repositories, two sites**. In this stage, each lesson had two
repositories serving parallel versions of their lessons websites: one using the
[styles infrastructure](https://carpentries.github.io/workbench/reference.html#styles),
and the other, a snapshot, using the [Workbench infrastructure](https://carpentries.github.io/workbench/reference.html#workbench).

For example, here is the state of the R for Social Scientists DataCarpentry lesson:


| version   | state    | site                                          | repository                                                                      |
| --------- | -------- | --------------------------------------------- | ------------------------------------------------------------------------------- |
| styles    | **live** | <https://datacarpentry.github.io/r-socialsci> | [datacarpentry/r-socialsci](https://github.com/datacarpentry/r-socialsci)       |
| Workbench | snapshot | <https://preview.carpentries.org/r-socialsci> | [fishtree-attempt/r-socialsci](https://github.com/fishtree-attempt/r-socialsci) |

In this stage of the beta phase, the community is encouraged to explore, fork,
and contribute to The Workbench version of these lessons in our
[sandbox GitHub organisation](https://github.com/fishtree-attempt). All of the
lessons in this repository are snapshots from the official lessons and any
changes made to them are strictly temporary, which means that this is a perfect
sandbox for practising your GitHub skills working with these sandboxed lessons. 

It is important to note that during this time, the Maintainers of these lessons 
will be focused on resolving and closing pull requests on the styles version,
so please be mindful before opening a pull request for these lessons, and open
an issue instead.

### Transition on 2023-02-06

In 20 days (Monday 2023-02-06), the the lessons currently in the beta phase will
enter the [second (beta) stage](https://carpentries.github.io/workbench/beta-phase.html#beta)
of the beta phase: **one repository, two sites.** 

Following the example above, the state of the R for Social Scientists DataCarpentry lesson will look like this:

| version   | state    | site                                          | repository                                                                | branch            |
| --------- | -------- | --------------------------------------------- | ------------------------------------------------------------------------- | ----------------- |
| styles    | locked   | <https://datacarpentry.github.io/r-socialsci> | [datacarpentry/r-socialsci](https://github.com/datacarpentry/r-socialsci) | `legacy/gh-pages` |
| Workbench | **live** | <https://preview.carpentries.org/r-socialsci> | [datacarpentry/r-socialsci](https://github.com/datacarpentry/r-socialsci) | `main`            |

The transition will use the following process:

1. A lesson release will be created for the styles version of the lesson
2. The default branch will be moved to have the prefix `legacy/` and locked from editing (only to be updated for crucial updates).
3. A [transformation of the default branch](https://github.com/carpentries/lesson-transition) will be set as `main` and that will become the default branch.

During this time, any changes to the lesson repository will only affect the
Workbench version of the lesson. Because the git history of the default branch
will be changing, **if you have a fork of one of these lessons, you must delete
it and re-fork if you want to make a new contribution**, otherwise, you 
[risk a failed pull request](https://carpentries.github.io/sandpaper-docs/pull-request.html#transition-from-carpentriesstyles).

After 8 weeks, the default lesson website will use The Workbench and the styles
branch will be removed from the GitHub repository.

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

Since 2022-12-21, 

 - [{sandpaper} version 0.11.3](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0113)
   - no updates :)
 - [{pegboard} version 0.3.2 -> 0.4.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-042)
   - A bug in parsing Jekyll templating syntax was fixed.
   - The minimum version of {tinkr} required is the current development version: 0.1.0.9000
 - [{varnish} 0.2.11 -> 0.2.13](https://carpentries.github.io/varnish/news/index.html#varnish-0213)
   - Table styling has been fixed so that tables are more accessible. They no
     longer have indentation in the first column, the headers are bold, rows are
     zebra striped, and the table is now accurately represented as a table for
     screen readers. 
   - The sidebar no longer takes up extra room at the foot of the document when
     collapsed. 
   <figure>
     <img src='{{ site.urlimg }}/blog/2023/01/dovetail-table-before.png' alt='screen capture of a simple table with the first column awkwardly indented, text not differentiated from headings, and no indication of even or odd rows' width="42%" style='border: solid 1pt black;'/>
     <img src='{{ site.urlimg }}/blog/2023/01/dovetail-table-after.png' alt='screen capture of a simple table with expected alignment, bold headings, and zebra striping that is much easier to look at' width="57%" style='border: solid 1pt black;'/>
     <figcaption>
     Before and after changes in {varnish}
     </figcaption>
   </figure>

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

One common practice for instructors is to fork a lesson to their own GitHub
account so that they can modify, rearrange, add, or omit episodes to serve their
audience. 

GitHub does not enable GitHub Actions or Pages by default, so there are a few
steps you need to do to make sure your fork can display a website.

1. (recommended) When creating your fork, you should **uncheck** "Copy the `main` branch only" checkbox.
![screenshot of the 'create a new fork' page with the "Copy the main branch only" checkbox highlighted in yellow]({{ site.urlimg }}/blog/2023/01/dovetail-fork-create.png)

2. To enable actions, on your fork, navigate to the actions tab, and click the button that says "I understand my workflows, go ahead and enable them".
<figure>
  <img src='{{ site.urlimg }}/blog/2023/01/dovetail-fork-actions-1.png' alt='screenshot of GitHub repository header showing that it is a fork with the "Actions" tab highlighted in yellow' style='border: solid 1pt black;'/>
  <img src='{{ site.urlimg }}/blog/2023/01/dovetail-fork-actions-enable.png' alt="screencapture with dialog that reads: Workflows aren't being run on this forked repository // Because this repository contained workflow files when it was forked, we have disabled them from running on this fork. Make sure you understand the configured owrkflows and their expected usage before enabling Actions on this repository. A green button as described above is below the text." style='border: solid 1pt black;'/>
  <figcaption>
  Enabling Github Actions in a fork
  </figcaption>
</figure>

3. To enable the pages, navigate to the "Settings" tab, click on "pages" on the
   side bar, and then set your site to deploy from the `gh-pages` branch.
<figure>
  <img src='{{ site.urlimg }}/blog/2023/01/dovetail-fork-pages-1.png' alt='screenshot of sidebar with the title "code and automation" with the last item, "pages", highlighted' width="30%" style='border: solid 1pt black;'/>
  <img src='{{ site.urlimg }}/blog/2023/01/dovetail-pages-deploy.png' alt="screenshot of GitHub pages form that shows the source as 'Deploy from a branch', the branch as 'gh-pages', the folder as 'root'" width="69%" style='border: solid 1pt black;'/>
  <figcaption>
  Enabling GitHub Pages in a fork
  </figcaption>
</figure>

