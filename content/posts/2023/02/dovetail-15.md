---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Stage 2 of the Beta Phase is Underway"
title: "The Dovetail #15: Updates from The Carpentries Workbench"
date: 2023-02-14
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the fifteenth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail) (our new lesson infrastructure).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 
If you are unfamiliar with The Workbench, you can [watch a video that describes
the workbench and the beta phase in two minutes](https://youtu.be/x7tETGpF3-4).

If you are interested in participating in discussions around The Carpentries
Workbench, or if you have questions, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

---

## Beta Phase Second Stage Is Live

The second stage of the beta phase is now live. This is a big milestone because
this is the portion of the beta phase where our community of contributors will
get a chance to interact with and use the Workbench in our live lessons before
we transition all of our lessons to use the new infrastructure in May 2023.

With this second stage of the beta phase, we have created a series of videos that
demonstrate some of the guides for what to expect during this period: 
[Workbench Beta Phase YouTube Playlist](https://www.youtube.com/playlist?list=PLXLapl_LKb4eQ3xOFHpYEb15HF3-7cMPO).

Here is the introduction to this stage of the beta phase: 

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/jnvEz-ojlUc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

On Monday, 2023-02-06, the beta phase lessons were transformed to
enter the [second (beta) stage](https://carpentries.github.io/workbench/beta-phase.html#beta)
of the beta phase: **one repository, two sites** where the Workbench version of
the lesson is the default for the lesson repository. 

For example, this is the state of the R for Social Scientists Data Carpentry lesson:

| version   | state    | site                                          | repository                                                                | branch            |
| --------- | -------- | --------------------------------------------- | ------------------------------------------------------------------------- | ----------------- |
| styles    | locked   | <https://datacarpentry.github.io/r-socialsci> | [datacarpentry/r-socialsci](https://github.com/datacarpentry/r-socialsci) | `legacy/gh-pages` |
| Workbench | **live** | <https://preview.carpentries.org/r-socialsci> | [datacarpentry/r-socialsci](https://github.com/datacarpentry/r-socialsci) | `main`            |

From now on, any changes to the lesson repository will only affect the
Workbench version of the lesson. Because the git history of the default branch
has changed, **if you have a fork of one of these lessons, you must [delete
it and re-fork if you want to make a new contribution](https://carpentries.github.io/workbench/faq.html#update-fork-from-styles)**, otherwise, you 
[risk a failed pull request](https://carpentries.github.io/sandpaper-docs/pull-request.html#transition-from-carpentriesstyles).

On Monday, 2023-04-03 the default lesson website will use the Workbench and the
styles branch will be removed from the GitHub repository.

### Thank You Beta Phase Participants

Being a Maintainer is not an easy job. As I mentioned in my ode to Maintainers
in dovetail 13, they are the quality assurance and moderators for our lessons
to ensure that they adhere to our teaching principles and provide guidance for
Instructors and learners. 

The Maintainers who are participating in the beta phase have gone above and
beyond to test out the Workbench and provide valuable feedback that could only
come from organic usage. It is because of the feedback from these Maintainers 
and other intrepid community members that the Workbench is stable. While not all
Maintainers have been able to participate in the beta stage due to extenuating
circumstances, I would like to thank them for stepping up despite the many false
starts that this project has encountered as we have battled our own extenuating
circumstances. 

With that, I would like to extend my thanks to the Maintainers of the beta phase
lessons: 

#### R for Social Scientists Maintainers

 - [jessesadler](https://github.com/jessesadler/)
 - [Juan F Fung](https://github.com/juanfung/)
 - [Eirini Zormpa](https://github.com/eirini-zormpa/)

#### Introduction to Geospatial Raster and Vector Data with R Maintainers

 - [drakeasberry](https://github.com/drakeasberry/)
 - [Ivo Agbor Arrey](https://github.com/arreyves/)
 - [Jemma Stachelek](https://github.com/jsta/)

#### Maintainers de Análisis y visualización de datos usando Python

 - [Irene Ramos](https://github.com/iramosp/)
 - [Agustina Pesce](https://github.com/aguspesce/)
 - [Vini Salazar](https://github.com/vinisalazar/)

#### Instructor Training Curriculum Maintainers

 - [Sarah M Brown](https://github.com/Brownsarahm/)
 - [Karen Word](https://github.com/karenword/)
 - [Tim Dennis](https://github.com/jt14den/)
 - [David Perez-Suarez](https://github.com/dpshelio/)
 - [Jon Wheeler](https://github.com/jonathanwheeler01/)
 - [Nathaniel Porter](https://github.com/ndporter/)
 - [Toby Hodges](https://github.com/tobyhodges/)
 - [Kelly Barnes](https://github.com/klbarnes20/)

#### R Ecology Lesson Maintainers

 - [François Michonneau](https://github.com/fmichonneau/)
 - [Tobias Busch](https://github.com/Teebusch/)
 - [Brian Seok](https://github.com/mondorescue/)

#### Library Carpentry Shell Lesson Maintainers

 - [Jamie Jamison](https://github.com/jmjamison/)
 - [Kaitlin Newson](https://github.com/kaitlinnewson/)
 - [annaoates](https://github.com/annaoates/)


I would also like to extend my sincere thanks to Saba Ferdous, Mark L Crowe,
Sarah Kaspar, Jennifer Stubbs, Athanasia M Mowinckel, Jannetta Styen, 
Sarah Stevens, and Philipp M Schäfer for their invaluable feedback, testing, and
general enthusiasm for the Workbench.


## Lessons Currently In the Beta Phase

The table below shows the status of lessons that are currently in the beta phase. 
All of these lessons are now in the [second (beta) stage](https://carpentries.github.io/workbench/beta-phase.html#beta) 
of the beta phase (one repository, two lesson websites).

| Lesson                                                   | Workbench URL                                                |
| -------------------------------------------------------- | ------------------------------------------------------------ |
| R for Social Scientists                                  | <https://preview.carpentries.org/r-socialsci>                |
| Introduction to Geospatial Raster and Vector Data with R | <https://preview.carpentries.org/r-raster-vector-geospatial> |
| Instructor Training                                      | <https://preview.carpentries.org/instructor-training>        |
| Análisis y visualización de datos usando Python          | <https://preview.carpentries.org/python-ecology-lesson-es>   |

[^1]: The Workbench Beta Phase is divided into three distinct stages, read more at <https://carpentries.github.io/workbench/beta-phase.html>.

## Updates to The Carpentries Workbench

Since 2022-01-17, 

 - [{sandpaper} version 0.11.3 -> 0.11.5](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0115)
   - a bug where the setup page was not added if it wasn't provisioned was fixed
   - The functions `update_cache()` and `pin_version()` will now work inside of
     subfolders. Thanks to Sarah Kaspar for spotting the bug
   - as of version 0.11.4, {sandpaper} now works with Pandoc version 3.
 - [{pegboard} version 0.4.2 -> 0.4.3](https://carpentries.github.io/pegboard/news/index.html#pegboard-043)
   - Improvements to link and image validation
     - alt-text validation better detects missing alt text (thanks to David P.S. for finding this)
     - an [allowed list of URL protocols has been created](https://carpentries.github.io/pegboard/reference/validate_links.html#external-links) to make sure that misspelled and malicious URL protocols are flagged.
 - [{varnish} 0.2.13 -> 0.2.14](https://carpentries.github.io/varnish/news/index.html#varnish-0214)
   - The "edit this page" links for beta stage lessons no longer redirects to
     the splash page.

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

One of the strengths of using the Workbench is that it gives you control over
the package cache used to build R-based lessons. For official Carpentries 
lessons, a [pull request to update the package cache](https://carpentries.github.io/sandpaper-docs/pull-request.html#updating-package-cache) 
will appear monthly and show you if there are any changes to the output of your 
lesson. 

For lessons that are not within one of The Carpentries GitHub organisations, you
can still update your package cache and create a pull request locally: open R in
your lesson directory and then use `sandpaper::update_cache()` to update the
package cache:

```r
> sandpaper::update_cache()                                                            
* (lesson-requirements) Project '.' loaded. [renv 0.16.0]
* Querying repositories for available source packages ... Done!
* Checking for updated packages ... Done!
* 4 packages have updates available.
→ Do you want to update the following packages?
# CRAN ===============================
- knitr       [1.41 -> 1.42]
- rmarkdown   [2.18 -> 2.20]
- xfun        [0.35 -> 0.37]
- yaml        [2.3.6 -> 2.3.7]

1: Yes
2: No

Selection: 1
```

When you do this, the packages will be updated in your lesson cache and the
file `renv/profiles/lesson-requirements/renv.lock` will be updated:

```
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   renv/profiles/lesson-requirements/renv.lock

no changes added to commit (use "git add" and/or "git commit -a")
```

You can now create a new branch, commit, and make a pull request to see what
changes happen in your lesson from the package updates.

This is also useful in [cases where cache invalidation has failed](https://github.com/carpentries/workbench/issues/40).
