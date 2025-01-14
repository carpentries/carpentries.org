---
layout: page
authors: ["Toby Hodges"]
teaser: "All lessons in The Carpentries Incubator will use our current lesson infrastructure by the end of 2025"
title: "Ending Support for _styles_ in the Incubator"
Date: 2025-01-14
time: "09:00:00"
tags: ["Curriculum", "The Carpentries Incubator", "The Carpentries Workbench"]
---

Our lesson infrastructure, [The Carpentries Workbench](https://carpentries.github.io/workbench/), was [rolled out](/blog/2023/08/celebrating-carpentries-workbench/) across all Data Carpentry, Library Carpentry, and Software Carpentry lessons in May 2023.
The Workbench replaced our previous lesson infrastructure, a [Jekyll](https://jekyllrb.com/)-based template (augmented by scripts and other resources developed by the community) affectionately known as _styles_.
The product of several years of work by [Zhian Kamvar](https://zkamvar.netlify.app/), the Workbench made a number of improvements over styles, e.g. by bringing lesson sites up to at least [WCAG AA standards](https://www.w3.org/WAI/WCAG2AA-Conformance) in web accessibility, and making local installation of the infrastructure significantly easier on most community members' systems.

![The Carpentries Workbench combines three R packages: sandpaper, pegboard, and varnish](/blog/2025/01/workbench-hex-collection.jpeg)

Since then, The Carpentries team has stopped maintaining the previous _styles_ infrastructure and [a documented transition workflow was published](https://carpentries.github.io/sandpaper-docs/migrating-from-styles.html) to help community members migrate their own lesson projects to use the Workbench.
The Carpentries Curriculum Team has been helping lesson developers with this process over the past 18 months, and community members, [Aleksandra Nenadic](https://github.com/anenadic) and [Matthew Bluteau](https://github.com/bielsnohr), facilitated a session to transition more lessons at [CarpentryConnect Heidelberg](https://biont-training.eu/CarpentryConnect2024.html) in November 2024.

The Carpentries supports the community's development of new lessons in [The Carpentries Incubator](https://carpentries-incubator.org/).
The Incubator hosts more than 150 of the community's lesson projects, from brand new lessons that are just getting started, through to polished and thoroughly-tested lessons that have been submitted for peer review in [The Carpentries Lab](https://carpentries-lab.org/).

These community-owned lessons use a mix of the old and new infrastructures: we estimate that 60 Incubator lessons are using the Workbench, which leaves a lot of projects that are using the unsupported _styles_ infrastructure.
To ensure that the Curriculum Team is able to support Incubator developers with their lessons -- and to help these developers take advantage of the improvements offered by the Workbench -- we will end support for the previous infrastructure in The Carpentries Incubator on 31 December, 2025.
**Any lesson repositories still using _styles_ in The Carpentries Incubator after the end of this year will be archived.**

## Supporting Workbench Transitions for Incubator Lessons
The process of migrating lessons from _styles_ to the Workbench is not straightforward, and many community members have found the workflow difficult and time consuming to set up and run without support.
Furthermore, since this is a process that only needs to be run once, the investment of time and effort may be too great for some.

In recognition of this, the Curriculum Team will support the transition of Incubator lessons to use the Workbench over the next 12 months.

### Workbench Transition Coworking Sessions
To help Incubator developers migrate their own lessons to the Workbench, the Curriculum Team will host monthly online Workbench Transition Coworking Sessions on the last Monday of each month. 
You can find the details of these sessions on [the community calendar](https://carpentries.org/community/events/) and [the Community Events Etherpad](https://pad.carpentries.org/community-sessions-2025).

Join these sessions to ask questions and get help with the process of migrating a lesson project/projects from _styles_ to the Workbench.

### Request help with a lesson transition
Alternatively, Incubator developers can ask the Curriculum Team to transition their lesson to the Workbench.
The team's capacity is limited so transitions may not happen quickly, but we will try to complete them as requested.
[Open an issue using the request form template](https://github.com/carpentries/lesson-transition/issues/new?assignees=tobyhodges&labels=&projects=&template=incubator-transition-request.yml&title=REQ%3A+) to ask the Curriculum Team to transition your lesson.
