---
layout: page
authors: ["Olexandr Konovalov"]
teaser: "An overview of the current state of the Ukrainian language localisation project initiated in 2022."
title: "Translating Software Carpentry lessons into Ukrainian language: a status update"
date: 2024-05-17
time: "09:00:00"
tags: ["Software Carpentry", "Internationalisation", "Equity and Inclusion", "Community"]
---

_This blog post was orginally published on Dr. Olexandr Konovalov's website as ["Software Carpentry for Ukraine: status update"](https://olexandr-konovalov.github.io/posts/2024/04/18/ukrainian-carpentry/). Minor modifications in style have been made to the original so that this version is in keeping with The Carpentries blog post conventions._  

-----------------------

This is an overview of the current state of the project of translating
Software Carpentry lessons into Ukrainian language. It accompanies the 
[slide of my lightning talk](https://zenodo.org/records/10995105) at the
[Collaborations Workshop 2024](https://www.software.ac.uk/workshop/collaborations-workshop-2024-cw24).

This project was initiated by me in summer 2022, and after getting some initial
practice with the translation toolchain in a small team, in 2023 we invited St Andrews students to join us under the 
[StARIS](https://www.st-andrews.ac.uk/students/academic/internships/staris/)
and [STEP](https://olexandr-konovalov.github.io/posts/2023/04/24/carpentries-step-up/)
programmes, and also [invited external contributors](https://olexandr-konovalov.github.io/posts/2023/03/28/carpentries-translation/).
By now the project involves 16 members from 6 locations, interacting via
a Slack workspace and regular monthly video calls.

We very much appreciated the ability to access the existing The Carpentries translation
infrastructure, which used the [Transifex](https://www.transifex.com/)
platform for collaborative translation (personal thanks to David Pérez-Suárez
for all the help with setup and rendering lessons). A pilot training in
version control with Git in Ukrainian took place at
[Research Software Camp: FAIR Software](https://www.eventbrite.co.uk/e/git-version-control-in-git-tickets-650799186887) in June 2023,
with its [recording available on YouTube](https://www.youtube.com/watch?v=RAaROljwy38).
However, while the training was delivered in Ukrainian, at that time
we still did not have a proper online version of the Git lesson in Ukrainian.

Continuing translation, by the start of 2024 we achieved further progress
with a few more lessons, most notably with the following four:
* [The Unix Shell](https://swcarpentry.github.io/shell-novice/)
* [Plotting and Programming in Python](https://swcarpentry.github.io/python-novice-gapminder/)
* [Introduction to R for Geospatial Data](https://datacarpentry.org/r-intro-geospatial/)
* [Programming with GAP](https://carpentries-incubator.github.io/gap-lesson/)

The image below shows the level of completion of the initial translation (green)
and its review (blue) for each lesson as it was in January 2024, just before we
started migration to another collaborative platform called [Crowdin](https://crowdin.com/).

![Transifex translation completion - January 2024]({{ site.urlimg }}/blog/2024/05/Transifex-2024-01-31.png)

The [Crowdin](https://crowdin.com/) platform offers better opportunities
for us, both in terms of its functionality and of the translation workflow,
with semi-automated rendering of the online version of the translated lesson
requiring only to press a few buttons in Crowdin and GitHub. In addition,
it will be already adapted to the most recent The Carpentries
lessons infrastructure, called the [Workbench](https://carpentries.github.io/workbench/). 
As soon as all the needed setup is implemented in The Carpentries
Crowdin organisation, we expect to provide online Ukrainian versions of
all translated lessons very soon. 

Right now we are ready to organise stand-alone trainings
in using version control with Git, and have already conducted a few.
The first online one in January 2024 was at the Winter School in System Analysis
and AI at Zaporizhzhia & Dnipro Polytechnics. For the first time, it
used the online lesson [Контроль версій за допомогою Git](https://ukrainian-carpentries.github.io/git-novice/) (Version control
with Git), and already using the new Workbench lesson infrastructure. (You can compare it with the [English version here](https://swcarpentry.github.io/git-novice/).)

This became possible thanks to the Bioconductor team letting us temporarily use their
Crowdin account, and personally thanks to Joel Nitta for exporting translations
from Transifex to Crowdin on a very short timescale. After the export, we
only had to manually migrate some text fragments, not picked up by the automated
procedure, and then approve all the remaining translations.

In March, another training was organised for the Ostroh Academy
(University of St Andrews' partner under the UK-Ukraine Twinning Initiative).
That was a hybrid event, with helpers present in the room
to respond to pink sticky notes when learners needed help. For the writeup and photos, visit
["В Острозькій академії відбувся весняний семінар комп'ютерної школи"](https://www.oa.edu.ua/ua/info/news/2024/06-03-01).

Furthermore, Zaporizhzhia Polytechnic is now using the Git lesson as a
foundation for one of the courses for the PhD students of the Department
of Computer Science and IT.

The next goal is having available online a full set of lessons for a standard
Python, R or GAP based Software Carpentry workshop. When at least one of these
three lessons on programming is completed, we would be ready to organise a full scale
Software Carpentry workshop (i.e. involving programming, UNIX shell and Git lessons)
for a Ukrainian-speaking audience, and start to build a community of Carpentries
Instructors in Ukraine. The translation of the Instructor Training curriculum is already
in progress. Please [contact me](https://olexandr-konovalov.github.io/about.html) if you're interested to learn more and take part
in this initiative!
