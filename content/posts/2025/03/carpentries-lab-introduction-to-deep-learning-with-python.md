---
layout: page
authors: ["Sven van der Burg", "Carsten Schnober", "Sarah M Brown", "Toby Hodges"]
teaser: "We are delighted to announce the addition of a new community-developed lesson on deep learning to The Carpentries Lab"
title: "The Carpentries Lab: Introduction to Deep Learning with Python"
date: 2025-03-11
time: "09:00:00"
tags: ["Curriculum", "Carpentries Lab", "Artificial Intelligence"]
---

We are delighted to announce the addition of [a new community-developed lesson on deep learning](https://carpentries-lab.github.io/deep-learning-intro/) 
to [The Carpentries Lab]({{< param lab_link >}}). The curriculum was [peer reviewed in the Lab Reviews repository](https://github.com/carpentries-lab/reviews/issues/25) 
and approved for inclusion in The Carpentries Lab on 6th February 2025.

The Carpentries Lab was set up as a space for peer-reviewed lessons developed by the community. Designed to 
complement [The Carpentries Incubator]({{< param incubator_link >}}), where the community collaborates on the 
development of new lessons on a wide range of topics, the Lab is intended to serve as a platform for open peer-review of 
these community-developed lessons and the hosting of lessons that have passed through that review process.


## **About the curriculum**

The use of deep learning has seen a sharp increase in popularity and applicability over the last decade. While deep
learning can be a useful tool for researchers from a wide range of domains, taking the first steps in the world of 
deep learning can be somewhat intimidating. 

Introduction to Deep Learning covers the fundamentals of deep learning in a practical and hands-on manner, for 
researchers who want to apply deep learning in their research. By the end of the course, students will be able to 
train their first neural network and understand the subsequent steps needed to improve the model.

The lesson can be taught in a 2-day or 4 half-day workshop.


![A section of the Introduction to Deep Learning lesson site, featuring a Python code block and the data visualisation it produces. The output visualisation is a plot with two lines, labelled “root_mean_squared_error” and “val_root_mean_squared_error”. The plot axes are labelled “epochs” and “RSME”.](/blog/2025/03/intro-dl-screengrab.png)
_Part of the [Monitor the training Process](https://carpentries-lab.github.io/deep-learning-intro/3-monitor-the-model.html) episode of the lesson._

### A brief history of the development of this lesson

What follows is a year-by-year history of the main contributors to the lesson. Of course, GitHub keeps the score, and all 
contributions to the commit history, big and, especially, small, can be better tracked 
[in this interactive contributor graph](https://github.com/carpentries-lab/deep-learning-intro/graphs/contributors). 
Over the years 30 people contributed to this lesson!

The development of the lesson started in 2020 in a collaboration between [Berend Weel](https://github.com/bpmweel) and 
[Florian Huber](https://github.com/florian-huber) (both at the Netherlands eScience Center at the time), 
[Peter Steinbach](https://github.com/psteinb), [Colin Sauze](https://github.com/colinsauze), 
[Samantha Wittke](https://github.com/samumantha), and [Toby Hodges](https://github.com/tobyhodges). 
During this period the main design of the lesson was drafted and the first pilot workshops were given.

During the year of 2021, Dafne van Kuppevelt, Djura Smits, and Sven van der Burg from the Netherlands eScience Center 
became involved and by the year 2022 Sven and Djura were the main contributors. In this period the lesson was taught a 
lot by various organisations and all feedback went into an ever-improving lesson.

In the period from 2023 till now the lesson was really polished towards its final shape, thanks to contributions from 
fresh team members Carsten Schnober and Pranav Chandramouli from the Netherlands eScience Center. This is the period that 
the lesson was transitioned to The Carpentries Workbench and went through The Carpentries Lab review process.


## **About the review process**

The curriculum was reviewed in [a public issue thread on The Carpentries Lab reviews repository](https://github.com/carpentries-lab/reviews/issues/25). 
This was a slightly unusual case because one of the authors is a member of The Carpentries Curriculum Team and was the 
sole Editor of the Lab at the time of submission. (Three other community members have joined as Editors since.) 
[Sarah M Brown](https://github.com/brownsarahm), formerly a long-standing member of the Trainers Leadership Committee, 
accepted an invitation to act as Guest Editor for this review. The authors and Carpentries team are enormously grateful 
to Sarah for the effort she put in and the diligence she displayed throughout the process. She made several essential 
contributions as Editor, in particular by encouraging the authors to more deeply explore the choice of example datasets 
used in the lesson (read more about this below). 

After the authors had responded to Sarah’s initial editorial checks, the curriculum was reviewed in detail by two 
volunteers from The Carpentries community: [Johanna Bayer](https://github.com/PaulaNietoG) and 
[Mike Laverick](https://github.com/mike-ivs) (thanks to Erin Becker for helping to connect Sarah with these reviewers). 
These reviewers were invited based on their expertise as Carpentries Instructors and their domain knowledge in machine 
learning and related fields.

The peer-review process led to a number of improvements to the accessibility of the lesson, with better alternative text 
descriptions for images and various adjustments to make language clearer and more beginner-friendly. The lesson was made 
easier to teach by other instructors through the addition and improvement of Instructor Notes, and the explanations of a 
number of important deep learning concepts were expanded. 

Perhaps most importantly, the Editor highlighted that one of the datasets used as an example in the lesson, the CIFAR-10 
dataset, is not available under a clearly-defined license. On closer inspection, the authors were surprised to find that 
CIFAR-10, a dataset very commonly used for benchmarking in machine learning research, was created with image files 
scraped from the internet without permission from their original owners. 

Sven van der Burg, one of the leading authors of the lesson, created [the “Dollar Street 10” dataset](https://zenodo.org/records/10970014) 
as an alternative to replace CIFAR-10 in the lesson. Dollar Street 10 is derived from the CC-BY-4.0 licensed Dollar 
Street Dataset from the Gapminder Project: a collection of images that has been more ethically assembled with an emphasis 
on ensuring that the data is representative of global diversity and accompanied by accurate metadata. The authors added a 
callout to the lesson to comment on this change, as they felt it represented a great entry point for a discussion of 
ethics in data and deep learning during a workshop.


## **Next steps**

The development team will of course keep on teaching this lesson at their institutes and keep on improving the lesson. We 
will have to, since deep learning is such a rapidly moving field. But our main goal is to help as many others as possible 
to adopt this lesson so that it can be taught around the world!

The lesson has been submitted to [The Journal of Open Source Education](https://jose.theoj.org/) for publication.

The wider Carpentries community can now [find the lesson in The Carpentries Lab](https://carpentries-lab.github.io/deep-learning-intro/), use and adapt it to teach their own workshops, contribute feedback, and suggest improvements. We hope you find it a helpful resource!


## Become a Reviewer

**The Carpentries Lab is looking for reviewers!** To volunteer to review a lesson in the Lab, please read [our Guide for Reviewers](https://github.com/carpentries-lab/reviews/blob/main/docs/reviewer_guide.md), and 
[register as a reviewer](https://forms.gle/cFD4nVjstTtVYoxg8) so we can contact you when relevant lessons are ready for 
review.

Lessons in the Incubator can be submitted for review in the Lab by [opening an issue on the reviews repository](https://github.com/carpentries-lab/reviews/issues/new?assignees=tobyhodges&labels=review&template=review_submission.yml&title=%5BReview%5D%3A+).


## **Acknowledgements**

We would like to thank all instructors and helpers that taught the course, and the community of people that left 
contributions to the project, no matter how big or small.

We also thank [Chris Endemann](https://github.com/qualiaMachine/) ([University of Wisconsin-Madison](https://www.wisc.edu/), US), 
[Nidhi Gowdra](https://nz.linkedin.com/in/nidhi-gowdra) ([University of Auckland](https://www.auckland.ac.nz/), 
New Zealand), [Renato Alves](https://github.com/unode) and 
[Lisanna Paladin](https://github.com/lisanna) ([EMBL Heidelberg](https://www.embl.org/sites/heidelberg/), Germany), 
who piloted this workshop at their institutes.

We thank The Carpentries for providing such a great framework for developing this lesson material.

We thank all students enrolled in the workshops that were taught using this lesson material for providing us with 
feedback.

Congratulations to the authors for creating an excellent lesson that will prove a useful resource to so many people:

* [Sven van der Burg](https://github.com/svenvanderburg)
* [Florian Huber](https://github.com/florian-huber/)
* [Peter Steinbach](https://github.com/psteinb/)
* [Colin Sauze](https://github.com/colinsauze/)
* [Carsten Schnober](https://github.com/carschno/)
* [Djura Smits](https://github.com/dsmits/)
* [Toby Hodges](https://github.com/tobyhodges/)
* [Berend Weel](https://github.com/bpmweel)
* [Pranav Chandramouli](https://github.com/cpranav93/)
* [Thor Wikfeldt](https://github.com/wikfeldt/)
* [Cunliang Geng](https://github.com/CunliangGeng/)
* [Chris Endemann](https://github.com/qualiaMachine/)
* [Giordano Lipari](https://github.com/wmotion/)
* [Samantha Wittke](https://github.com/samumantha)
* [Ashwin V. Mohanan](https://github.com/ashwinvis)
* [Sarah Stevens](https://github.com/sstevens2)
* [axdy-a](https://github.com/axdy-a)
* [YL Wang](https://github.com/code4yonglei)
* [Maurice de Kleijn](https://github.com/Morrizzzzz)
* [Laura Ootes](https://github.com/laurasootes)
* [Dominik Kutra](https://github.com/k-dominik)
* [Yi Sun](https://github.com/sunyi000)
* [Lucas Esclapez](https://github.com/esclapez)
* [Renato Alves](https://github.com/unode)
* [Miguel A Magaña](https://github.com/miguel-mx)
* [Fenne Riemslagh](https://github.com/FenneRiemslagh)
* [Dafne van Kuppevelt](https://github.com/dafnevk)
* [Anne Fouilloux](https://github.com/annefou)

And huge thanks again to [Sarah M Brown](https://github.com/brownsarahm) for acting as Guest Editor, and to the 
reviewers, [Johanna Bayer](https://github.com/likeajumprope) and [Mike Laverick](https://github.com/mike-ivs).
