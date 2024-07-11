---
layout: page
authors: ["Toby Hodges"]
teaser: "Everything you need to get involved and make Carpentries lessons easier to teach."
title: "The 2023 Instructor Notes Drive Starts Next Week!"
date: 2023-05-06
time: "09:00:00"
tags: ["Curriculum", "Community", "Workbench", "Lessons"]
---

[The 2023 Instructor Notes Drive](https://carpentries.org/blog/2023/04/instructor-notes-drive-announcement/)
will take place from 8th to 19th May.
During these two weeks, we call on the community to help us expand, update, and improve
the guidance provided to Instructors on Carpentries lessons.
It is a great opportunity to make an impact on the effectiveness of Carpentries lessons,
to learn more about how to contribute to lessons,
and to practice and develop your skills working with Markdown, Git, and GitHub.


## Who can get involved in the Drive?

**Instructors with experience teaching any 
Data Carpentry, Library Carpentry, or Software Carpentry lesson** 
are particularly well-suited to contribute to the Instructor Notes Drive.
But this event is open to anyone in the community who wants to get involved:

* Instructors can share their experience by 
  adding new Notes and making sure existing Notes are up-to-date
* Anyone who knows how to edit a Markdown file and open a pull request with GitHub 
  can help by
  relocating existing Notes to the place where they are most relevant in a lesson
* Anyone who does not yet have these Markdown/GitHub skills can
  watch [the instructional videos](#more-detailed-instructions) 
  and/or follow [the written instructions](https://docs.google.com/document/d/1HCvnxPWulAzIFrRSe3GdRHOKERDSoufyatwYz5TxMxk/edit?usp=sharing)
  (see below)
  to learn what they need to contribute to the Drive.
* Everyone can join one or more of the [scheduled coworking sessions](#coworking-sessions) to
  ask questions and collaborate with the Curriculum Team and other community members 
  on the Instructor Notes alongside other community members.


## How to edit Instructor Notes

To suggest updates, improvements, additions, and other changes to
the Instructor Notes of a Carpentries lesson,
open a pull request on the relevant lesson repository.
(If you do not yet know how to do this,
check out the [_More Detailed Instructions_](#more-detailed-instructions) section below.)

**General Instructor Notes** for a lesson are stored in 
the `instructors/instructor-notes.md` file of a lesson repository.
Any guidance that applies to the lesson as a whole,
as opposed to being specific to a particular section/exercise/element,
should be added to that source Markdown file.

Notes that will make most sense to Instructors 
when viewed alongside a particular part of the lesson
should be added as **inline Instructor Notes**.
These can be placed in the source file of the relevant episode
(stored in the `episodes/` folder of the lesson repository)
as [a _fenced div_][workbench-docs-fenced-divs]:

```
::::::::::::::::: instructor

A fenced div with the 'instructor' keyword will appear as an inline Instructor Note, 
visible only in the Instructor View of the lesson website.

::::::::::::::::::::::::::::

```

### More Detailed Instructions

To help those still learning to use GitHub to edit files,
and/or who need more context for following the instructions above,
we have prepared a couple of short videos:

1. [Editing the Instructors Notes page of a lesson](https://youtu.be/UL1Zd8Ivjg8)
2. [Adding an inline Instructor Note to a lesson](https://youtu.be/mGHZwb28Cwo)


We also provide [a set of more detailed written Instructions](https://docs.google.com/document/d/1HCvnxPWulAzIFrRSe3GdRHOKERDSoufyatwYz5TxMxk/edit?usp=sharing) that include
step-by-step instructions for contributors to follow.

## One Instructor Note: one pull request

To make contributions easier for lesson Maintainers to review, 
**we recommend that you make individual pull requests for changes to individual Instructor Notes**. 
For example, if you want to add two new Instructor Notes, open two separate pull requests to suggest each one.
If you want to move several Instructor Notes to become inline Notes in the lesson,
open a separate pull request to suggest moving each one.


## Coworking sessions

The Curriculum Team will host six Coworking Sessions over the course of the
Instructor Notes Drive.
These will provide a space for community members to contribute to the Drive
together, giving us a chance to better coordinate our efforts, ask questions
and learn from each other. 
You can find connection details for these sessions, 
and add your name if you plan to attend,
[in the relevant Etherpad](https://pad.carpentries.org/instructor-notes-drive-coworking-2023).

The following coworking sessions are scheduled for the 2023 Instructor Notes Drive:

1. [**9th May 2023, 10:00 UTC**](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Coworking%3A+Instructor+Notes+Drive+2023&iso=20230509T10&p1=%3A&ah=1), hosted by Toby Hodges
2. [**11th May 2023, 00:00 UTC**](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Coworking%3A+Instructor+Notes+Drive+2023&iso=20230511T00&p1=%3A&ah=1), hosted by Erin Becker
3. [**12th May 2023, 14:00 UTC**](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Coworking%3A+Instructor+Notes+Drive+2023&iso=20230512T14&p1=%3A&ah=1), hosted by Toby Hodges
4. [**16th May 2023, 08:00 UTC**](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Coworking%3A+Instructor+Notes+Drive+2023&iso=20230516T08&p1=%3A&ah=1), hosted by Toby Hodges
5. [**18th May 2023, 00:00 UTC**](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Coworking%3A+Instructor+Notes+Drive+2023&iso=20230518T00&p1=%3A&ah=1), hosted by Erin Becker
6. [**19th May 2023, 12:00 UTC**](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Coworking%3A+Instructor+Notes+Drive+2023&iso=20230519T12&p1=%3A&ah=1), hosted by Toby Hodges

([Check out these events in The Carpentries Community Calendar](https://carpentries.org/community/#community-events).)


## What contributions are most needed, and where?

All Carpentries lessons have room for improvement, and all contributions are welcome - from fixing typos to adding whole new Instructor Notes!

If you would like more guidance towards places where particular types of contribution could be most impactful,
please take a look at [the Collaboration Sheet](https://docs.google.com/spreadsheets/d/1UEo5be8-jadaDoduWS5ssTGXtYmfzT9uIV6dugiZyLQ/edit?usp=sharing), which includes a column suggesting the type(s) of
contribution most needed for each lesson.
(You are welcome to make contributions beyond these suggestions - 
they are intended as a guide only.)

Finally a note that Data Carpentry's [_Data Analysis and Visualization in Python for Ecologists_][dc-ecology-python] lesson - 
and the Spanish translation, [_Análisis y visualización de datos usando Python_][dc-ecology-python-es] -
includes exercise solutions in its Instructor Notes page.
In addition to the contributions welcome on all lessons, there is a need to relocate these solutions to their respective challenges
within the episodes of the lesson. Pull requests to help with that effort will be very welcome!


If you have any questions about the Instructor Notes Drive,
please [contact Toby Hodges](mailto:tobyhodges@carpentries.org).

[dc-ecology-python]: https://datacarpentry.org/python-ecology-lesson/
[dc-ecology-python-es]:https://datacarpentry.org/python-ecology-lesson-es/
[video-general-instructor-notes]: FIXME
[video-inline-instructor-notes]: FIXME
[workbench-docs-fenced-divs]: https://carpentries.github.io/sandpaper-docs/episodes.html#callout-blocks
