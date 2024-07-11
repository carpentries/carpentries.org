---
layout: page
authors: ["Mike Trizna", "Jen Thomas", "Reinder Radersma", "Adriana De Palma", "Sichong Peng", "Michael Culshaw-Maurer", "Toby Hodges", "Erin Becker"]
teaser: "Trialing a reimagined version of the popular Data Carpentry lesson: Data Analysis and Visualization in R for Ecologists."
title: "Beta Testing an Alternative Version of R Ecology lesson"
date: 2023-07-10
time: "09:00:00"
tags: ["Curriculum", "Data Carpentry", "Carpentries Incubator"]
---

The Data Carpentry: Ecology Curriculum Advisory Committee has approved 
[a redesigned version of the _Data Analysis and Visualization in R for Ecologists_ lesson][r-ecology-alt]
for beta testing.
[Curriculum Advisors][curriculum-advisors] invite the Data Carpentry community to 
**teach this alternative version of the lesson and provide feedback**,
to inform their discussions as they consider formally adopting it and replacing the [current version in the curriculum][r-ecology-current].


## About the Redesigned Lesson
The lesson was redesigned and developed by [Michael Culshaw-Maurer][mcm]
in [The Carpentries Incubator][incubator]
during his tenure in The Carpentries Curriculum Team
as a post-doc at [CyVerse][cyverse].

The redesigned lesson teaches the same fundamental skills in data handling, analysis, and visualisation
as the current Data Carpentry lesson,
but the narrative structure and key packages used are notably different.

![Overview of the redesigned lesson content]({{ site.urlimg }}/blog/2023/07/2023-07-10-r-ecology-alt-beta-overview.svg)

After orienting learners to R and RStudio 
and motivating them to adopt a scripting approach to data analysis,
the lesson aims to keep the audience motivated by
leading swiftly into an exploration of `ggplot2` for visualisation.
Having given learners [a taste of the cake][ccmcr19-keynote],
the remaining episodes are designed to guide them through 
the ingredients - the fundamentals of loading data and working with data frame objects and other data types in R -
and the instructions - using packages from the _tidyverse_ to filter, process, summarise, and otherwise manipulate data for analysis and visualise -
of the recipe.

![Screenshot of the 'Changing Labels' section of the redesigned version of the Data Carpentry R Ecology lesson]({{ site.urlimg }}/blog/2023/07/2023-07-10-r-ecology-alt-beta-screenshot.png)
_A screenshot of one section from the second episode of the redesigned lesson._

After initial development was completed, 
the lesson was alpha tested by Michael at a workshop at Rice University,
and taught again by Susan Washko and Jessica Guo at a workshop at the University of Arizona.
After these successful trials, and several updates to the lesson in response to feedback received at the workshops,
Michael presented the lesson to the Curriculum Advisory Committee in April this year.
The committee is now considering whether to formally adopt the lesson 
as a replacement for the version currently used in the Data Carpentry Ecology curriculum. 

One potentially important change, which Curriculum Advisors are particularly keen to collect feedback on,
is the omission of [content on interacting with relational databases from R][r-ecology-sql]
that exists in the current version of the lesson.
We are looking forward to receiving feedback from Instructors who teach this alternative version of the lesson
on whether or not they felt the absence of this content 
and would be keen to see it reintroduced to the lesson.


## The Beta Testing Phase
To help Curriculum Advisors make an informed decision about adoption of the redesigned lesson,
the committee is now calling for Instructors to teach it and share their feedback.

**If you are already planning to teach a Data Carpentry R Ecology workshop,
why not use this lesson instead of the official equivalent,
and share Instructor and Learner feedback?
Or maybe this is just the excuse you have been looking for to schedule a workshop?**

If you do plan to teach the lesson, 
please send an email to [the Curriculum Team](mailto:curriculum@carpentries.org) 
and [DC Ecology CAC](mailto:curriculum-advisors-ecology@lists.carpentries.org) 
to tell them about it.
If possible, The Carpentries and/or the CAC would love to send someone to observe these pilot workshops.

### How to submit feedback
Feedback on the quality and effectiveness of the redesigned lesson is essential for the CAC to take next steps.

Feedback from Instructors and Learners would be gratefully received: 

- by email to [the Curriculum Advisors](mailto:curriculum-advisors-ecology@lists.carpentries.org)
- by opening an issue using [the _Pilot Workshop Feedback_ template issue form][pilot-workshop-feedback-issue]
on [the lesson repository in The Carpentries Incubator][r-ecology-alt-repo].
- Pull requests to that repository are also welcome:
  [James Azam][james] has kindly volunteered to maintain this repository 
  in addition to his role as one of the Maintainers of the official DC R Ecology lesson - Thanks, James!

### Next Steps
If the Curriculum Advisors receive sufficient feedback on the lesson
(feedback from a minimum of two workshops will be required, but more is desirable),
the committee will review that feedback and consider whether to formally adopt it,
replacing the current version in the Data Carpentry Ecology curriculum.


[ccmcr19-keynote]: https://www.youtube.com/watch?v=fQ4t7p6ZXDg
[curriculum-advisors]: https://carpentries.org/curriculum-advisors/
[cyverse]: https://www.cyverse.org/
[incubator]: https://carpentries-incubator.org/
[james]: https://github.com/jamesmbaazam
[mcm]: https://www.michaelc-m.com/
[pilot-workshop-feedback-issue]: https://github.com/carpentries-incubator/R-ecology-lesson-alternative/issues/new?assignees=&labels=type%3Adiscussion&projects=&template=pilot_workshop_feedback.yml&title=%5BPilot+workshop+feedback%5D%3A+
[r-ecology-alt]: https://carpentries-incubator.github.io/R-ecology-lesson-alternative/
[r-ecology-alt-repo]: https://github.com/carpentries-incubator/R-ecology-lesson-alternative
[r-ecology-current]: https://datacarpentry.org/R-ecology-lesson
[r-ecology-sql]: https://datacarpentry.org/R-ecology-lesson/05-r-and-databases.html
