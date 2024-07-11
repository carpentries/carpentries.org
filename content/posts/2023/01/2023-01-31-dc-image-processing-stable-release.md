---
layout: page
authors: ["Toby Hodges"]
teaser: "Announcing the stable release of a new curriculum teaching image processing skills. Sign up to host a workshop today!"
title: "Launching Data Carpentry: Image Processing with Python"
date: 2023-01-31
time: "09:00:00"
tags: ["Curriculum", "Data Carpentry"]
---

I am thrilled to announce the first official release of the new Data Carpentry curriculum,
[_Image Processing with Python_][dc-image].
In November 2022, the Curriculum Advisory Committee met and approved a motion 
to move the lesson out of _beta_ testing and into _stable_ status.
Version 1.0.0 of the curriculum was [published to Zenodo][dc-image-zenodo] last week.
This means the curriculum is now available for teaching in official Data Carpentry workshops.


## Curriculum Content
The _Image Processing with Python_ curriculum teaches the concepts and skills needed to 
write automated processing pipelines for image data.
Using examples from morphometrics, 
the curriculum covers the steps of a typical image processing workflow: 
loading images, masking, blurring and thresholding data, and ends with 
a capstone challenge to provide a chance for additional practice.
Like [_Foundations of Astronomical Data Science_][dc-astro], released in April 2022,
this curriculum consists on a single lesson, designed to be taught over two full days
or four half-days.

The curriculum uses a variety of example images that do not require any domain-specific knowledge. 
However, it does require learners to have gained some familiarity with the Python programming language,
such as by attending 
a [Software Carpentry][swc], 
[Data Carpentry: Ecology][dc-ecology] or 
[Data Carpentry: Social Sciences][dc-socsci] workshop.


## Want to Teach the Curriculum?
_Image Processing with Python_ can now be taught in self-organised and
centrally-organised Data Carpentry workshops.
Set up your own workshop, or make sure you are subscribed to
[the `instructors` TopicBox list][topicbox-instructors]
to hear about opportunities to teach the lesson.

Some of the lesson Maintainers hosted [an Instructor Onboarding session][dc-image-instructor-onboarding]
at CarpentryCon@Home 2022, which you can watch on [The Carpentries YouTube channel][carpentries-youtube].


## Host a Data Carpentry: Image Processing Workshop
You can now [request a workshop][cow-request-form] teaching 
the _Image Processing with Python_ curriculum from The Carpentries,
or [organise and host your own][sow-registration-form].
We are expecting high demand for these workshops,
and Centrally-Organised workshops (those administered by The Carpentries) 
will initially be limited in number while we assess 
the Instructor community's capacity for teaching this new curriculum. 
The Workshop Administrator will work with every request on a case by case basis. 


## Curriculum Background and Acknowledgments
The lesson was originally developed for
[the _Digital Imaging and Vision Applications in Science (DIVAS)_][divas] project,
where it was taught to undergraduates majoring in natural science.
This initial lesson design and development was led by 
Prof. Mark Meysenburg, Prof. Tessa Durham Brooks, Dr. Raychelle Burks, Dr. Erin Doyle and colleagues
at Doane University, Nebraska, USA,
and used `cv2`, the Python interface to [_OpenCV_][opencv],
as its main toolkit for image processing.

In an effort led by Dominik Kutra and Dr. Constantin Pape of
[the European Molecular Biology Laboratory (EMBL)][embl],
the lesson was then converted to use [_scikit-image_][skimage] as the primary library,
and was taught in alpha pilots at EMBL and [The University of Arizona][uaz].

In June 2021, Dr. Kimberly Meechan, David Palmquist, Prof. Ulf Schiller, and Dr. Robert Turner answered 
[a call for volunteers to help make these changes to the curriculum][call-for-contributors],
and this group has done excellent work to prepare the lesson for a beta release.

In May 2022, we published [a call for beta pilots][call-for-beta-pilots] to help polish the curriculum and 
ensure it was ready to be taught by The Carpentries global Instructor community.
Answering this call, [the University of Würzburg][uwü] and [the Earlham Institute][ei]
hosted beta pilot workshops and provided feedback and improvements to the lesson repository.

The first Curriculum Advisory Committee for Data Carpentry: Image Processing was established
shortly after that call for beta pilots was published,
and includes members with experience and expertise in image processing from a wide range of
domains.
The members of the CAC are:

- Ulf Schiller (Chair)
- Josh Moore (Secretary)
- Marianne Corvellec
- Erick Martins Ratamero
- Sunil Shende

The current Maintainer team is:

- [Toby Hodges](https://github.com/tobyhodges)
- [Kimberly Meechan](https://github.com/k-meech)
- [David Palmquist](https://github.com/quist00)
- [Ulf Schiller](https://github.com/uschille)
- [Robert Turner](https://github.com/bobturneruk)

It has been a long road for this curriculum to get to this point,
where we can finally make a stable release and share it with the Instructor community.
I am so grateful to all the people mentioned above, 
and to the many other community members who have contributed to the project along the way.
If you have taught the lesson, hosted a workshop for the curriculum,
opened an issue or pull request in [the repository][dc-image-repo], 
or shared the lesson site with a friend or colleague, 
**thank you!**
Additional thanks go to my colleagues in the Curriculum Team,
Erin Becker and Zhian Kamvar,
for the role they have played in the development of the curriculum and the preparations for its release.
I am excited to see what the Data Carpentry community does with the curriculum from here,
and how it evolves in the coming years.


[call-for-beta-pilots]: https://carpentries.org/blog/2022/05/image-processing-beta-announcement/
[call-for-contributors]: https://carpentries.topicbox.com/groups/discuss/Ta8ff359298db95c6-M390cec7393b29ed4b74bdda5/looking-for-contributors-maintainers-for-image-processing-with-python-lesson
[carpentries-youtube]: https://www.youtube.com/channel/UCBOUNBBZxc4DML3F89cEvGA
[cow-request-form]: https://amy.carpentries.org/forms/request_workshop/
[dc-astro]: https://datacarpentry.org/astronomy-python/
[dc-ecology]: https://datacarpentry.org/ecology-workshop/
[dc-image]: https://datacarpentry.org/image-processing/
[dc-image-instructor-onboarding]: https://www.youtube.com/watch?v=_0cR3x5onh8
[dc-image-repo]: https://github.com/datacarpentry/image-processing
[dc-image-zenodo]: https://zenodo.org/record/7576952#.Y9gV1eLMKM8
[dc-socsci]: https://datacarpentry.org/socialsci-workshop/
[divas]: https://web.doane.edu/Colleges-Divisions-Programs/College-of-arts-sciences/Science-Mathematics-and-information-science-and-technology/Biology-Department/Divas-Project
[ei]: https://www.earlham.ac.uk/
[embl]: https://bio-it.embl.de/
[opencv]: https://opencv.org/
[skimage]: https://scikit-image.org/
[sow-registration-form]: https://amy.carpentries.org/forms/self-organised/
[swc]: https://software-carpentry.org/lessons/
[topicbox-instructors]: https://carpentries.topicbox.com/groups/instructors
[uaz]: https://new.library.arizona.edu/
[uwü]: https://www.uni-wuerzburg.de/startseite/
