---
layout: page
authors: ["Toby Hodges", "Zhian N. Kamvar"]
teaser: "Final preparations are underway"
title: "The Dovetail #17: Updates from The Carpentries Workbench"
date: 2023-04-13
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the seventeenth post in [a series that we are calling "The Dovetail",
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

## Lesson Transitions Have Begun

Since [the beta phase ended on 3rd April](https://carpentries.org/blog/2023/04/workbench-beta-phase-complete/), the first four lesson transitions have been completed. The remaining lessons will transition to use the Workbench by early May, but you may see some lessons making the switch before then. We are coordinating with lesson Maintainers to schedule early transitions where possible, to help keep the rollout on track.

As with any wholesale transition of infrastructure, this process is not easy or without disruption, but we have been putting safeguards in place for the community. For example, each lesson transition will be accompanied by:

- [A preview of the Workbench version of the lesson](https://fishtree-attempt.github.io/OpenRefine-ecology-lesson/), for Maintainers to verify before the final transition occurs
- An [automated transition process](https://github.com/carpentries/lesson-transition#readme) that minimises downtime and user-error for lesson repositories
- A protected main branch 
- [A templated message with instructions for replacing invalidated pull requests](https://github.com/carpentries/lesson-transition/blob/main/close-pr-msg.md)


## Join a Community Discussion

Zhian will be hosting two community discussions about the Workbench on Monday 17th April. The sessions are taking place at [14:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Carpentries+Community+Discussion&iso=20230417T1400) and [22:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Carpentries+Community+Discussion&iso=20230417T2200) - click on the links to see those in your local timezone. 

These sessions are an opportunity to learn more about the new infrastructure, ask any questions you have - from the perspective of an Instructor, Maintainer, lesson contributor, lesson developer, or any other role in the community - and to hear about the experiences of other community members who have been working with the Workbench.

To sign up to attend, please add your details in the relevant section of [the community-discussions etherpad](https://pad.carpentries.org/community-discussions).


## Maintainer Onboarding

A round of Maintainer Onboarding is taking place this month, which will include a session designed to orientate participants to the new infrastructure. If you are curious to learn more about how the Workbench transition will affect lesson Maintainers, take a few minutes to browse through [the Transition Guide](https://carpentries.github.io/workbench/transition-guide.html#for-maintainers).


## Processing Outstanding Pull Requests

One impact of the infrastructure transition is that any open pull requests on lesson repositories will be invalidated when the change takes place. To avoid this, **Maintainers are working hard to process outstanding pull requests on their lesson repositories this month**. You can expect to see plenty of activity on GitHub. If you were planning to submit a change to a Data Carpentry, Library Carpentry, or Software Carpentry lesson, **we recommend that you wait until after the transition has taken place before you open any new PRs**.

Huge thanks go to all of the Maintainers who are devoting extra time and effort to help prepare for this transition. This process is particularly demanding for the Maintainer community, and we realy appreciate the cooperation and positivity that we have received from them.


## Updates to The Carpentries Workbench

Since 2023-03-09, 

 - [{sandpaper} version 0.11.8 -> 0.11.15](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-01115-2023-04-05)
   - broken glossary links have been fixed
   - the default CONTRIBUTING.md has been updated
   - a 404 page has been implemented
   - `sandpaper::serve()` now works with a path argument
   - various fixes for {renv} versions 0.17.0 through 0.17.2 (red queen dynamics) 
 - [{pegboard} version 0.4.3 -> 0.5.2](https://carpentries.github.io/pegboard/news/index.html#pegboard-052-2023-04-05)
   - validators no longer truncate on GitHub Actions
   - validators will now run on ALL markdown files in the lesson, not just episode content
 - [{varnish} version 0.2.14 -> 0.2.16](https://carpentries.github.io/varnish/news/index.html#varnish-0216)
   - carpentries-lab logo has been updated

To update your local Workbench installation, open R and use the following code:

```r
# Enable repository from carpentries
options(repos = c(
  ropensci = 'https://carpentries.r-universe.dev',
  CRAN = 'https://cloud.r-project.org'))
# Download and install sandpaper in R
install.packages(c('tinkr', 'pegboard', 'sandpaper', 'varnish'))
```


