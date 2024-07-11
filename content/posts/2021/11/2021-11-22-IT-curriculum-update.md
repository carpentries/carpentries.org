---
layout: page
authors: ["Karen Word"]
teaser: "The new version of the Instructor Training curriculum has been released"
title: "The Carpentries Instructor Training Curriculum has been Updated!"
date: 2021-11-22
time: "09:00:00"
tags: ["Instructor Trainers"]
---


Throughout 2021, The Carpentries Core Team and Trainer community have been developing, discussing, and testing an updated version of our [Instructor Training curriculum](https://carpentries.github.io/instructor-training). It has now been merged into our [repository on GitHub](https://github.com/carpentries/instructor-training) and submitted to   [Zenodo](https://zenodo.org/record/5709383) for official release!

### Changes in this update include:
* General changes to make the curriculum more useable and maintainable:
    - Reduced hyperlinks to external websites 
    - Eliminated use of handouts for activities
    - Reduced content on Carpentries policies; increased orientation to main sources of policy information
    - Reduced use of jargon
    - Reduced use of coding in examples to accommodate variable background knowledge
    - Structural changes to improve timing and flow, allowing for more consistent breaks & alternate schedules
* Content removed or transferred to [optional exercises page](https://carpentries.github.io/instructor-training/additional_exercises/index.html) (more relevant to lesson development, which is now a separate curriculum)
    - Practice writing multiple choice questions
    - Practice writing learner profiles
    - Content on Bloom's Taxonomy
* Content changed or rearranged
    - Previous episode on "Mindset" reduced and combined with ["Motivation and Demotivation" episode](https://carpentries.github.io/instructor-training/08-motivation/index.html)
    - Previous content on Equity, Inclusion, and Accessibility in "Motivation and Demotivation" episode moved to [its own episode](https://carpentries.github.io/instructor-training/09-eia/index.html) and expanded
    - Previous references to formative assessment sprinkled across episodes are now highlighted as distinct uses
    - Mental models are now [explained using concept mapping](https://carpentries.github.io/instructor-training/02-practice-learning/index.html) and analogies
    - Some strategies specific to teaching in-person are now presented with suggested adaptations for teaching online
    - Content on [Instructor Checkout](https://carpentries.github.io/instructor-training/checkout/index.html) is consolidated and clarified
* Added or enhanced content
    - Concluding a workshop (added to [content on introductions](https://carpentries.github.io/instructor-training/23-introductions/index.html))
    - [Team teaching practices](https://carpentries.github.io/instructor-training/21-management/index.html), reinforcing common mechanics of Carpentries workshops


### Goals reserved for the next update (not included yet):
* Improvements to referencing (to replace previous use of hyperlinks)
* Further improvements to new episode on EIA as well as additional bonus content on this topic (we have [a grant and some awesome partners](https://carpentries.org/blog/2021/06/carpentries-sloan-foundation-announcement/) to help; please get in touch if you would like to be involved!)
* Additional suggestions related to online or hybrid instruction. (These will continue to evolve separately, with content migrating into our core curriculum as needed/ requested by our community.)


## Why Change a Good Thing?
Given the positive feedback we regularly receive on our program, you may be wondering why we would do anything more than minor maintenance! 

As with all Carpentries curricula, our Instructor Training curriculum receives feedback from our community as it is used. 
Some of this can be responded to promptly with minimal disruption to routine instruction. However, broader revisions that involve rearrangement of content across episodes cannot be implemented bit by bit while our curriculum is in use. In addition, substantive changes that influence how our Instructor Trainers teach need to be carefully communicated to avoid last-minute surprises during preparation or instruction. Work on changes like these is concentrated in the periods prior to version release. The last major update for this lesson was in 2018. 

## How Do You Update a Curriculum In Use?
For this update we used a GitHub account under The Carpentries umbrella, called "data-lessons". Working in a [fork](https://github.com/data-lessons/instructor-training) allowed us to separate comments on the lesson-in-development from those in the existing lesson. Changes were submitted as pull requests to the data-lessons repository, reviewed and merged there; the primary branch of that repository was used in a [pull request to our main repository](https://github.com/carpentries/instructor-training/pull/1215), which was then subjected to broader community review. Meanwhile, the [fully rendered curriculum](https://data-lessons.github.io/instructor-training/) in the data-lessons repository could be field tested with minimal disruption.

This workflow was not entirely satisfactory. One effect was to narrow the audience for early conversations, which occurred in the "quieter" data-lessons repository and was mostly restricted to Maintainers and a few Trainers who were paying close attention. Some found this process to be too isolated, preferring that all conversation remain in our main repository. In addition, the many ways to provide feedback (issues or comments on the PR in the main repository; issues or comments on PRs in data-lessons) proved confusing for both contributors and maintainers. 

## When is it "Done"?

<blockquote class="twitter-tweet">
<p lang="en" dir="ltr">I just merged a PR that closed over 40 issues. from the command line bc github couldn&#39;t resolve merge conflicts in browser. That was probably the scariest line I&#39;ve ever run from a terminal.</p>&mdash; Dr. Sarah M Brown (@BrownSarahM) <a href="https://twitter.com/BrownSarahM/status/1455956325901475840?ref_src=twsrc%5Etfw">November 3, 2021</a>
</blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

Maintenance is a big job in this repository, and there is always more to do! The wonderful thing about the Instructor Training curriculum is that it gets a lot of attention. For new and prospective Instructors, it is the launch point for their relationship with The Carpentries, Trainers study it regularly as they prepare to teach, and many community-members find themselves referencing it when they teach workshops or just want to share favorite tidbits with a friend or colleague. In a collaborative community, this leads to a lot of great suggestions! This update addressed more than 40 outstanding issues in addition to feedback delivered in Trainer meetings and other contexts. Yet, more remain. In the end, it was time to release this curriculum when we had a new version that had been through testing and feedback and seemed to be meeting our minimum standard of "better than the last one" in most respects.

## What Comes Next?
In the coming weeks we will be doing some cleanup to identify issues that we still plan to address and decide which others to close. It is always a hard choice to close an issue without resolving it! At The Carpentries, we [value all contributions](https://carpentries.org/values/). The value of a contribution is not necessarily evident in its implementation, however; it may instead serve to provoke thought that ultimately leads to work along different lines, or it may serve to draw out opposing arguments or identify sticky trade-offs. Hard choices like these are an important role of Maintainers to focus conversation and prioritize effort. 

The Carpentries Instructor Trainer community will also be having a conversation about curriculum maintenance, led by our [Trainers Leadership](https://github.com/carpentries/trainers/blob/main/governance.md) group, to evaluate the potential for more diverse roles in maintenance for this repository. For example, this lesson houses things like checkout policy, but contributions that address policy fall outside the typical duties of curriculum upkeep. By spreading out our maintenance efforts among Trainers with specific leadership interests, we hope to make routine maintenance more manageable and narrow the focus of work during update periods.

A few of our goals for that next update are already clear, because they are priorities that we had hoped to address but ultimately had to cut from this release! We are excited about pursuing new and better ways of citing the many resources pointed out to us by our community members along with the primary and secondary literature upon which our curriculum rests. We are also looking forward to further development of content on Equity, Inclusion, and Accessibility, with an eye towards evidence-based practices and maximum impact in our short-format context. Finally, as our community continues to learn and grow through creative implementation of online workshops, we will be looking to identify ways in which we can support new Instructors in preparing to embrace the challenges and opportunities of teaching online.

## Thank you!!
As always, this work would not have been possible without the dedicated participation of our community, especially our community of Instructor Trainers, and most particularly our community Maintainers, Sarah Brown and Tim Dennis, whose counsel and support have been indispensible in maintaining forward progress and bringing this project to a close. We are also grateful to the Chan Zuckerberg Initiative for funding that supports the Instructor Training efforts of The Carpentries Core Team, allowing us to take on the more intensive writing and coordinating work that cannot reasonably be performed by volunteers.

Forty eight people have made contributions via GitHub that were incorporated since our last release. These are: Karen Word; Maneesha Sane; Kelly Barnes; Sarah M Brown; François Michonneau; Christina Koch; Rayna M Harris; Erin Becker; Brian Ballsun-Stanton; Gerard Capes; Toby Hodges; Serah Njambi; Sarah Stevens; Zhian Namir Kamvar; Angela Li; Ariel Deardorff; Pradeep Eranti; SherAaron Hurt; Aleksandra Nenadic; Eric Jankowski; Dr. Kari L. Jordan; Laurent Heirendt; Murray Cadzow; Aaron Tran; Alec L. Robitaille; Alexander James Ball; Bianca Peterson; Christa de Kock; Daniel Chen; Darya P Vanichkina; Pérez-Suárez; Elizabeth McAulay; George Milunovich; GIUSEPPE PROFITI; Hugo Gruson; Jeffrey Oliver; Jonah Duckles; Juvonen, Matti; Konrad U. Förstner; Lex Nederbragt; Liz Stokes; Martin Stoffers; Michael Black; Michael Henry; Neal Davis; Sarah Peter; Sichong; Tong Liang; Ashwin Vishnu Mohanan. Contributions to this curriculum come in many forms, and we are further grateful to all those whose efforts in testing, discussion, and other feedback have guided its development! 

## Looking for more?
If you are excited about The Carpentries Instructor Training curriculum, you might want to consider becoming a Carpentries Instructor Trainer! [Applications are open now through December 2, 2021](https://carpentries.org/blog/2021/11/Trainer-Training-open/).

## Citation

The Carpentries Instructor Training, November 2021. Word K., Brown S.M., Dennis T., Barnes K. (eds). DOI: [10.5281/zenodo.5709383](https://doi.org/10.5281/zenodo.5709383).

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5709383.svg)](https://doi.org/10.5281/zenodo.5709383)
