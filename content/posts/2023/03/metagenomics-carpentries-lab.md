---
layout: page
authors: ["Toby Hodges", "Claudia Zirión Martínez", "Diego Garfias Gallegos", "Aarón Espinosa Jaime", "José Abel Lovaco Flores", "J Abraham Avelar Rivas", "Tania Vanessa Arellano Fernández", "Edder Daniel Díaz", "Luis Gerardo Tejero Gómez", "Nelly Sélem Mojica"]
teaser: "A peer-reviewed Metagenomics curriculum has been added to The Carpentries Lab"
title: "The Carpentries Lab: Metagenomics Curriculum"
date: 2023-03-28
time: "09:00:00"
tags: ["Curriculum", "The Carpentries Lab"]
---

We are delighted to announce the addition of [a new community-developed curriculum on Metagenomics][metagenomics-overview] to 
[The Carpentries Lab][lab-home]. The curriculum was [peer reviewed in the Lab Reviews repository][review-thread] and approved for inclusion in 
The Carpentries Lab on 24th February 2023.

The Carpentries Lab was set up as a space for peer-reviewed lessons developed by the community. Designed to complement [
The Carpentries Incubator][incubator-home], where the community collaborates on the development of new lessons on a wide range of topics, the Lab is 
intended to serve as a platform for open peer review of these community-developed lessons and the hosting of lessons that have passed through that 
review process.

## About the curriculum

The Metagenomics curriculum is intended to be used by anyone interested in conducting microbiome research with metagenomics analysis. The curriculum 
starts with basic recommendations on working with bioinformatics and data-based projects, and it teaches from scratch the programming skills required 
to do these kinds of projects. Here you will learn the language bash with enough depth to navigate the filesystem, edit files from the command line, 
automate tasks with scripts, and run programs. You will also learn the basics of the R language to analyse data using special libraries and make graphs. 
These skills will allow you to conduct a complete metagenomics workflow, from sequencing reads to diversity analysis, using a standard pipeline and giving 
you the tools to explore more of the available programs and build your own workflow. 

This curriculum was created by undergrad and graduate students and researchers who were having a hard time knowing where to start on their metagenomics 
project. They joined forces to put together a comprehensive workflow and decided to share it with the rest of the struggling scientists in the world.

## About the review process

The curriculum was reviewed in [a public issue thread on The Carpentries Lab `reviews` repository][review-thread]. After some initial editorial checks, 
the curriculum was reviewed by two volunteers from The Carpentries community: [Paula Nieto Garcia][paula-github] and [Fotis Psomopoulos][fotis-github]. 
These reviewers were invited based on their expertise as Carpentries Instructors and their domain knowledge in metagenomics and related fields.

The peer-review process enhanced the lesson by rearranging and breaking down several episodes, making them more connected and reducing the cognitive load. 
It improved the software setup by making it easier to install in a wider range of settings, and the instructions were simplified in a way that made them 
easier to maintain. Over all of the episodes, the reviewers helped with the clarity of the contents and the distribution and delivery of the exercises by 
making them more helpful for practice and a self-evaluation of the contents learned.

The review process allowed the authors to make sure that the lessons were understandable and fluent from a fresh perspective. The reviewers were 
attentive to detail, corroborated that the code works as intended, and proposed changes that were in line with the author's intention. The editor's list 
of requirements helped them understand what was important to include and put more attention to, such as the accessibility of the pages and figures. 
The reviewer's comments were added at each point of the editor's checklist, which was useful for understanding the context of the comment, but it may be 
easier to address the comments in a list of issues in the lesson's repository and mention them in the corresponding point of the checklist. Each issue 
could have the comment and the proposed change along with a label of the priority of the changes.

## Next steps

The authors intend to use the lesson for formal undergrad courses in bioinformatics and independent workshops. They will also use the experience that 
this lesson development gave them to create more curricula on new topics and have more ideas to expand the Metagenomics curriculum in the future.

The wider Carpentries community can now find these lessons in The Carpentries Lab, use and adapt them to teach their own workshops, contribute feedback, 
and suggest improvements:

* [Metagenomics Workshop Overview][metagenomics-overview]
* [Project Organization and Management for Metagenomics](https://carpentries-lab.github.io/metagenomics-organization/)
* [Introduction to the Command Line for Metagenomics](https://carpentries-lab.github.io/metagenomics-shell/)
* [Introduction to R](https://carpentries-lab.github.io/metagenomics-R/)
* [Data Processing and Visualization for Metagenomics](https://carpentries-lab.github.io/metagenomics-analysis/)

**The Carpentries Lab is looking for reviewers!** To volunteer to review a lesson in the Lab, please read [our Guide for Reviewers][reviewer-guide], 
and [register as a reviewer][reviewer-volunteer-form] so we can contact you when relevant lessons are ready for review.

Lessons in the Incubator can be submitted for review in the Lab by [opening an issue on the `reviews` repository][new-review-issue].

## Acknowledgements

We are very grateful to everyone who helped make this first review in The Carpentries Lab a success. The authors would like to thank Karina Enriquez 
Guillén and Rafael Pérez Estrada for their valuable contributions while testing the lessons.

Congratulations to the authors for creating an excellent curriculum that will prove a useful resource to so many people:

* Claudia Zirión Martínez
* Diego Garfias Gallegos
* Aarón Espinosa Jaime
* José Abel Lovaco Flores
* J Abraham Avelar Rivas
* Tania Vanessa Arellano Fernández
* Edder Daniel Díaz
* Luis Gerardo Tejero Gómez
* Nelly Sélem Mojica

And huge thanks to the reviewers, who devoted a significant amount of time to reviewing the lessons, and exemplified the communication, diligence, 
and expertise required for a successful peer review process:

* Paula Nieto Garcia
* Fotis Psomopoulos


[fotis-github]: https://github.com/fpsom
[incubator-home]: https://carpentries-incubator.org/
[lab-home]: https://carpentries-lab.org/
[metagenomics-overview]: https://carpentries-lab.github.io/metagenomics-workshop/
[new-review-issue]: https://github.com/carpentries-lab/reviews/issues/new?assignees=tobyhodges&labels=review&template=review_submission.yml&title=%5BReview%5D%3A+
[paula-github]: https://github.com/PaulaNietoG
[review-thread]: https://github.com/carpentries-lab/reviews/issues/11
[reviewer-guide]: https://github.com/carpentries-lab/reviews/blob/main/docs/reviewer_guide.md
[reviewer-volunteer-form]: https://forms.gle/cFD4nVjstTtVYoxg8
