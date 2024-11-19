---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Prepare for transition to The Workbench in May"
title: "Workbench Beta Phase Complete"
date: 2023-04-04
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta"]
---


## Beta Phase Complete

Since October 2022, we have been running a test of our new lesson infrastructure,
known as [The Workbench](https://carpentries.github.io/workbench).
If you are unfamiliar with The Workbench, you can [watch a video that describes
the workbench and the beta phase in two minutes](https://youtu.be/x7tETGpF3-4).
If you are interested in participating in discussions around The Carpentries
Workbench, or if you have questions, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

Today, when you visit any of these lessons, you will be presented with a
version that is built using The Carpentries Workbench.

| Lesson                                                   | Workbench URL                                          |
| -------------------------------------------------------- | ------------------------------------------------------ |
| R for Social Scientists                                  | <https://datacarpentry.org/r-socialsci>                |
| Introduction to Geospatial Raster and Vector Data with R | <https://datacarpentry.org/r-raster-vector-geospatial> |
| Análisis y visualización de datos usando Python          | <https://datacarpentry.org/python-ecology-lesson-es>   |
| Instructor Training                                      | <https://carpentries.github.io/instructor-training>    |


## Workbench Transition to happen in May 2023

The beta phase was a success,
and we can now begin final preparations for a full rollout of the new infrastructure.
In May 2023, we will transition all of our official lessons to use The Workbench.
This transition will do two things:

1. transform the file structure and syntax to The Workbench
2. clean the Git history to accurately reflect lesson-specific commits.

The transition process is automated in
[carpentries/lesson-transition](https://github.com/carpentries/lesson-transition#readme)
and lesson Maintainers will have the opportunity to audit the transformed
lessons before the changes are finalised. A list of lessons and their transformation
status can be found at <https://github.com/carpentries/lesson-transition/issues/23>.

### Avoid making pull requests until May

Because the transition will significantly change the folder structure and clean
the Git history, it is important to avoid making pull requests to the lessons 
in April. The reason for this is that after the transition, any old forks will
be invalid and cannot be used to contribute. 

If you have made a contribution to our lessons in the past and want to do so in
the future, you will need to [delete and re-fork your fork of the lesson](https://carpentries.github.io/workbench/faq.html#update-fork-from-styles).
Below is a video that describes the process in under four minutes and then 
demonstrates what can happen if you do not delete your fork. 

<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/9DVwy818MIE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


### Feature freeze until May

Because we are now out of Beta, but not yet deployed to all of our lessons, The
Workbench will be in a feature freeze until May. This means that if you request
new features in The Workbench, you will have to wait until May at the earliest to see the
implementations.

## Thank You

Thanks to the feedback provided by Maintainers, Trainers, Instructors, and
Learners during the beta phase of The Workbench, we have been able to
continuously improve on the experience in teaching and developing lessons. 

And as always, [thank you beta phase
participants](https://carpentries.org/blog/2023/02/dovetail-15/#thank-you-beta-phase-participants)
for your dedication to trying out The Workbench.

