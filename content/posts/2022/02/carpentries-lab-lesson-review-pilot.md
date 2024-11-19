---
layout: page
authors: ["Michael Culshaw-Maurer", "Toby Hodges"]
teaser: "The Carpentries will start publishing peer-reviewed lessons in The Carpentries Lab."
title: "Piloting Open Peer Review of Lessons"
date: 2022-02-07
time: "09:00:00"
tags: ["Curriculum", "The Carpentries Lab"]
---

For the past few years, The Carpentries curriculum community has been designing and developing lessons in [The Carpentries Incubator][incubator]. As illustrated by the first figure in [Zhian Kamvar, Lesson Infrastructure Technology Developer's post from last year, about alpha testing the infrastructure redesign][lesson-infra-post], this lesson development is now happening at a huge scale. At the time of writing, the Incubator hosts more than [100 lessons][community-lessons] at various stages of the development cycle. We have been supporting these efforts by [providing training on lesson development][ldsg1-retrospective], highlighting the ways community members can contribute to the development of lessons in a regular series of [Incubator Lesson Spotlight posts on this blog][incubator-posts], and maintaining channels for this subcommunity of lesson developers to communicate and collaborate.

Today, we are thrilled to announce the next step towards ensuring our community members receive credit for creating high-quality, open-source lessons.

**[The Carpentries Lab][lab] is a space for lessons that have passed through peer review.** Community-developed lessons are eligible for submission to The Carpentries Lab when they reach a state where they can be used by anyone familiar with The Carpentries teaching methods and sufficiently knowledgable on the lesson subject matter. The single lesson currently published in The Carpentries Lab, [Python for Atmosphere and Ocean Scientists][pyaos-lesson], which was reviewed and accepted at [the Journal of Open Source Education (JOSE)][jose], is a great example of what we are aiming to collect there.

In the coming weeks, we will begin piloting a process of open peer review for lessons developed by our community, for acceptance into The Carpentries Lab. We are delighted to collaborate with JOSE on this effort, so that lesson authors will have the option to submit their lesson for publication at the journal after passing through The Carpentries Lab review process.

A sibling journal to [the Journal of Open Source Software (JOSS)][joss], JOSE publishes articles that describe open source materials and software tools for educational use. It is an entirely volunteer-led initiative, and a very good fit to the aims we have for open lesson review. Our hope is that, by providing a way for authors to improve their lessons and received authorship credit for their work, we can reward the time and effort our community members have put into producing a lesson that is ready to be re-used by others.

JOSE are looking for volunteers to become reviewers. This provides a good opportunity for members of The Carpentries community to support the project and gain valuable experience in an open review process. [To volunteer as a reviewer at JOSE, you can fill out this form][jose-reviewer-registration].

The primary purpose of the peer review process will be to improve the quality of the lessons submitted. In The Carpentries Lab, feedback from editors and reviewers will focus on the design of the lesson, the value of its challenges as tools for formative assessment, the accessibility of the content, and the support provided to Instructors who wish to teach it in a workshop. The review process will be coordinated by members of [The Carpentries Curriculum Team][curriculum-team] and reviewers will be members of The Carpentries community wherever possible. Reviews will take place as publicly-visible issue threads on [the GitHub repository][reviews-repo], in a system inspired by [ROpenSci's open peer review of software][ropensci-review].

To indicate to other community members that accepted lessons have undergone this process and met the standard expected, authors will receive a badge and banner for use in their lesson repository and pages respectively, a new URL under <https://carpentries-lab.org/>, and be listed in The Carpentries Lab community on Zenodo. If authors opt to also submit the lesson to JOSE, they will need to write a short paper to accompany the lesson. This will be reviewed at JOSE and, if it is accepted, the lesson and paper will receive [a CrossRef DOI][crossref] and be published in the journal. Authors can read more about [what is required for lessons to be reviewed and accepted at JOSE in their online documentation][jose-submission-info].

In the coming weeks, we will be reaching out to authors of lessons in The Carpentries Incubator to invite submissions to The Carpentries Lab. During this intial pilot phase, we will commit only to reviewing those lessons that are invited to submit. Watch this space for our reflections on these early reviews and updates on the next phase of this new program!

If you are interested in learning more about lesson development with The Carpentries, check out the #lesson-dev channel on The Carpentries Slack, or stop by one of our [monthly co-working sessions][coworking-codimd].


[community-lessons]: https://carpentries.org/community-lessons/
[coworking-codimd]: https://codimd.carpentries.org/lessondev-coworking
[crossref]: https://www.crossref.org/
[curriculum-team]: https://carpentries.org/core-team-projects/#curriculum-team
[incubator]: https://carpentries-incubator.org/
[incubator-posts]: https://carpentries.org/posts-by-tags/#blog-tag-carpentries-incubator
[jose]: https://jose.theoj.org/
[jose-reviewer-registration]: https://jose.theoj.org/reviewer-signup.html
[jose-submission-info]: https://openjournals.readthedocs.io/en/jose/submitting.html#how-to-prepare-a-learning-module-submission
[joss]: http://joss.theoj.org/
[lab]: https://carpentries-lab.org/
[reviews-repo]: https://github.com/carpentries-lab/reviews/
[ldsg1-retrospective]: https://carpentries.org/blog/2021/06/ldsg1-retrospective/
[lesson-infra-post]: https://carpentries.org/blog/2021/07/infrastructure-testing/
[pyaos-lesson]: https://carpentries-lab.github.io/python-aos-lesson/
[ropensci-review]: https://github.com/ropensci/software-review
