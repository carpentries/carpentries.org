---
layout: page
authors: ["Toby Hodges"]
teaser: "What we learned from the inaugural round of lesson development training."
title: "Reflecting on the first round of Lesson Development Study Groups"
date: 2021-06-02
time: "09:00:00"
tags: ["Curriculum Development"]
---

In February-April 2021, we ran the inaugural round of [Lesson Development Study Groups (LDSG)][ldsg-announcement-post]. The program combined weekly group discussions with reading and practical "homework" tasks requiring participants to apply the skills and practices they were learning to their lesson as they developed it.

[The Study Groups program][study-groups] was designed to help community members taking the first steps in designing a new lesson in [The Carpentries Incubator][incubator]. It focussed on good practices in lesson design, and elements of The Carpentries lesson infrastructure, with the aim of giving the participants a solid foundation from which to continue building their lessons. We also hoped that it would help us to identify gaps in the resources we provide around lesson development, as we work to improve the quality and accessibility of our infrastructure, processes, and documentation.

## What was the format?

In this first round, 28 participants worked through the program in four groups, working on 18 lessons. Reading tasks during the program largely focussed on **The Carpentries [Curriculum Development Handbook][cdh]** and **Greg Wilson's [Teaching Tech Together][ttt]**, supplemented with sections of [**the Instructor Training curriculum**][it]. Homework tasks were designed to give participants an opportunity to put the theory they were reading into practice while they designed and developed their lessons.

Teaching a lesson for the first time is a vital _intermediate_ step in the process of lesson development so, in addition to the other applied lesson development tasks, the program included a break for participants to teach a section of the lesson in a "trial run," coming back together afterwards to reflect on the experience as a group.

The participants were supported by [Group Facilitators](#gratitude), volunteers from the community with experience in lesson development and maintenance.


## What worked?

In feedback collecting during and after the round, participants indicated that they appreciated the format of weekly group discussions, with a rotating Discussion Lead role taken by a different group member each time. This kind of regular contact provided an "accountability framework" and motivation to remain engaged with the lesson development process every week, and the Lead role gave everyone a chance to gain experience facilitating a group discussion.

Participants made significant progress on their lesson, with 12 of 19 feedback survey respondents reporting that they had almost finished or completely finished writing exercises and explanatory text for at least one episode at the end of the ten week round.

From an internal perspective, the feedback received and discussions observed helped us to identify areas where our documentation and guidance for lesson developers can be improved. For example, many Study Groups participants found it challenging to identify an appropriate example data set for their lesson. They could have been better served by a section in the Curriculum Development Handbook recommending repositories of openly licensed data, data sets already used in other lessons, and a rubric to use when choosing between several different options.


## What would we do differently next time?

An application process was necessary for the Study Groups program, to try to ensure that participants shared common goals as they entered the program, e.g. all working to begin new lessons so that they could engage with every step of the design process. However, applications were not filtered based on prior experience with the tools used for lesson development in The Carpentries - GitHub, Markdown, etc - or some of the concepts and terms introduced in Instructor Training - cognitive load, formative assessment, mental models, etc. This resulted in a very different experience for participants depending on their previous familiarity with The Carpentries.

The combination of learning lesson design skills with learning the technical skills required to create a lesson website resulted in cognitive overload for a number of participants and should be avoided in future iterations. In the future we will be clearer about the prerequisites, and/or provide opportunities to learn the required skills before joining the training.


## What did we learn?

From the moment we began reviewing applications for this LDSG round, it was clear that members of The Carpentries community have great ideas for lessons and an enthusiasm for teaching complex concepts and technical skills to new audiences. Lessons like [an Introduction to Artificial Intelligence for GLAM (Galleries, Libraries, Museums, and Archives) staff][ai-glam] and [Time Series Analysis of Solar Power Generation Data][ts-solar] are a clear demonstration of the potential for our community to bring training and an increased awareness to domains that have a growing need for computational research skills.

Participants' experiences in the LDSG program reiterated that the current lesson template has a steep learning curve, and that it can be challenging to set up a local system for Jekyll to provide preview builds of lesson sites. [These issues are already known][lesson-template-redesign-post] and the experience of Study Groups participants provide further evidence of the need for new ways to create and build our lessons.

We also observed that lesson development is easier to do when you are not alone. The Study Groups participants that worked collaboratively with others on a lesson tended to make more progress over the course of the round, and many others reported the benefits of a regular opportunity to connect and share experiences with others going through the same process. This experience has strengthened our resolve to focus future training on _collaborative_ lesson development skills: future LDSG rounds, and similar training in other formats (see below) should encourage participation from groups working on the same lessons, and teach people how to collaborate effectively as well as how to design and write a good lesson.

Finally, the volume of applications and interest in the program demonstrated the appetite our community has for training on this topic but the ten-week Study Groups format is perhaps not best suited to scale up
and meet that demand.


## What is coming next?

Encouraged by the enthusiasm and success of the participants in the inaugural LDSG round, we are continuing to develop training material on this topic. We hope to produce a curriculum that combines and expands on elements of [the Curriculum Development Handbook][cdh], [the Lesson Example pages][lesson-example], [the Study Groups reference pages][study-groups], [Teaching Tech Together][ttt], and [The Carpentries Instructor Training][it], referring to the scientific literature behind the concepts and approaches promoted in those resources. When developing this curriculum, and working on our tools and resources for lesson development more generally, we will continue to incorporate the feedback we receive from the community via the Study Groups and through other channels. Please open an issue on [the Study Groups repository][ldsg-repo] or
[send me an email][toby] if you want to talk about this more.

We intend to trial that curriculum in a shorter format training, more similar to our two-day Instructor Training workshops, to explore an alternative to the multi-week LDSG setup. We anticipate some downsides to adopting this shorter format - principally the loss of the accountability and structure offered to participants by meeting regularly over multiple weeks, and of the space those meetings provided for discussion among participants - but the potential upsides - increased scalability, a format that fits more easily into people's schedules, pulling diverse resources into a single curriculum, decreased organisational and administrative overheads - make it worth exploring.


## Gratitude

Huge thanks to the Group Facilitators who volunteered time each week to support the
Study Groups:

- Tim Dennis
- Kate Hertweck
- Mateusz Kuzak
- Aleksandra Nenadic
- Sarah Stevens
- Yuka Takemon

and to the following people who provided ideas and support at various stages of the process:

- Kelly Barnes
- Serah Njambi Kiburu
- Malvika Sharan
- Allegra Via
- Greg Wilson
- Karen Word

[ai-glam]: https://carpentries-incubator.github.io/machine-learning-librarians-archivists/
[cdh]: https://cdh.carpentries.org/
[incubator]: https://carpentries.org/community-lessons/
[it]: https://carpentries.github.io/instructor-training/
[ldsg-announcement-post]: https://carpentries.org/blog/2020/12/lesson-development-study-groups/
[ldsg-repo]: https://github.com/carpentries-incubator/study-groups/
[lesson-example]: https://carpentries.github.io/lesson-example/
[lesson-template-redesign-post]: https://carpentries.org/blog/2020/08/lesson-template-design/
[study-groups]: https://carpentries-incubator.github.io/study-groups/
[toby]: mailto:tobyhodges@carpentries.org
[ts-solar]: https://carpentries-incubator.github.io/data-management-pipelines-engineering/index.html
[ttt]: https://teachtogether.tech/
