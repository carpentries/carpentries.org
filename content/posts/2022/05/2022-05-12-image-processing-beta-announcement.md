---
layout: page
authors: ["Kimberly Meechan", "David Palmquist", "Ulf Schiller", "Robert Turner", "Toby Hodges"]
teaser: "Host or teach a pilot workshop with a brand new Data Carpentry curriculum"
title: "Image Processing with Python - Call for Beta Pilot Applications"
date: 2022-05-19
time: "09:00:00"
tags: ["Curriculum", "Pilot Workshops"]
---

The [Data Carpentry: _Image Processing with Python_][lesson] curriculum is ready for beta testing.
First developed for [the _Digital Imaging and Vision Applications in Science (DIVAS)_][divas] project,
the lesson has already been through several iterations and pilot workshops.
The curriculum is now ready for testing by the Instructor community,
with the goal of preparing a full release within the next 12 months.

**We are seeking community members to host and teach beta pilot workshops 
with the _Image Processing with Python_ curriculum in July - October 2022.**
Continue reading for more information on the curriculum, 
the previous alpha pilot workshops, 
and how to apply to host and/or teach a beta pilot.

## About the Lesson

The [Data Carpentry: _Image Processing with Python_][lesson] curriculum teaches
the fundamental concepts and skills needed to load, edit, and analyse image data
with the Python programming language.
Like the recently-released [_Foundations of Astronomical Data Science_][dc-astro] curriculum,
_Image Processing with Python_ is composed of a single lesson, 
designed to be taught over a two-day workshop.

Aimed at learners who are already familiar with the basics of Python -
the skills that may be learned by attending another Software or Data Carpentry workshop -
the lesson explores:

* how images are stored digitally, 
* how these files can be loaded and represented in Python,
* how to select and edit regions in an image,
* how to handle noise in image data,
* how to select pixels in an image based on their properties, and
* how to automatically identify and analyse objects within an image.

The curriculum uses [the _scikit-image_ library][skimage] to teach these skills,
and is designed to be taught within a [Jupyter][jupyter] environment.
The lesson includes many different example images, 
including plants, bacterial colonies, and household objects,
which are intended to be accessible to learners from a diverse range of backgrounds.

## Lesson Development and Pilot workshops

The lesson was originally developed for
[the _Digital Imaging and Vision Applications in Science (DIVAS)_][divas] project,
where it was taught to undergraduates majoring in natural science.
This initial lesson design and development was led by 
Prof. Mark Meysenburg, Prof. Tessa Durham Brooks, Dr. Raychelle Burks, and colleagues
at Doane University, Nebraska, USA,
and used `cv2`, the Python interface to [_OpenCV_][opencv],
as its main toolkit for image processing.

In an effort led by Dominik Kutra and Dr. Constantin Pape of
[the European Molecular Biology Laboratory (EMBL)][embl],
the lesson was then converted to use _scikit-image_ as the primary library,
and was taught in alpha pilots [at EMBL][alpha1] and [The University of Arizona][alpha2].

Feedback collected at these pilots suggested that the curriculum teaches skills
that learners found valuable,
and introduced concepts that are vital to building expertise in image processing.
Learner responses and notes taken by observers at the alpha pilots
highlighted the need for several changes to lesson content and structure.
These included a reorganisation of introductory content 
to provide more opportinities for hands-on learning early in the workshop, 
and the use of a different image viewer tool for inspecting data throughout the lesson.

In June 2021, Dr. Kimberly Meechan, David Palmquist, Prof. Ulf Schiller, and Dr. Robert Turner answered 
[a call for volunteers to help make these changes to the curriculum][call-for-contributors],
and this group has done excellent work to prepare the lesson for a beta release.


## Apply to Host/Teach a Beta Pilot

Beta pilot workshops are the first time a new lesson is taught by Instructors 
who are not its authors.
The beta phase is vital for the continuing improvement of this lesson,
to ensure that the curriculum is ready to be offered for centrally-organised workshops.
It provides The Carpentries with valuable information about
whether a curriculum can be taught by any certified Instructor who has the relevant domain knowledge,
with a reasonable amount of time to prepare.
Beta pilot workshops also tell us how accessible the lesson content and supporting information is for learners
in a range of communities and regions.

**Help us take the curriculum to the next level,
by volunteering to host or teach an _Image Processing with Python_ beta pilot workshop.**

Beta pilot instructors should:

* Be certified Instructors with The Carpentries and have taught at least 2 Carpentries workshops.
* Should not yet have made any major contribution to the lesson.
* Have experience working with image data in Python.

Beta pilot Instructors commit to:

* Participating in 1-2 hours of onboarding led by lesson developers prior to their workshop. Every effort will be made to offer this onboarding asynchronously as well as synchronously.
* Teaching the material over 2 full days or 4 half days of instruction (~10-12 hours instructional time) in July - October 2022 (exact dates to be determined).
* Advertising to and recruiting appropriate learners. Learners for this workshop should have experience with Bash shell and Python programming equivalent to that taught in a Software Carpentry Python workshop (the lesson includes [a detailed list of the prerequisite skills in Python and Bash][prereq-list]).
* Providing feedback to the lesson developer(s) after their workshop to enable the lesson to be further polished in final preparation for an official release.

**If you would like to host a pilot of the lesson at your institute/organisation, please [fill out this short application form for beta pilot hosts][application] before the end of Friday 27 May 2022 ([anywhere on Earth][AoE])**. The information collected there will help us coordinate the pilot process and maximise the impact of the process on the lesson material.

If you are an Instructor interested in teaching a pilot workshop for the curriculum, but cannot commit to hosting the workshop yourself, please contact [Toby Hodges](mailto:tobyhodges@carpentries.org).

If you have any questions about the lesson and the beta pilot process, please contact [Toby Hodges](mailto:tobyhodges@carpentries.org).

## Acknowledgements

The Carpentries is very grateful to everyone who has contributed to bringing the lesson to the point of a beta release.

* Special thanks to Prof. Mark Meysenburg, Prof. Tessa Durham Brooks, Dr. Raychelle Burks, and everyone involved in the initial design and testing of the curriculum within [the DIVAS Project][divas].
* Dominik Kutra and Dr. Constantin Pape made an essential contribution by converting the lesson to use _scikit-learn_. 
* Dominik Kutra and Dr. Gregor Mönke taught the alpha pilot at EMBL, with help from Dr. Christian Tischer and support from [the EMBL Bio-IT Project][embl-bio-it].
* Trisha Adamus and Prof. Mark Meysenburg taught the alpha pilot at [the University of Arizona][uoa], with help from Zuzana Adams, Amirhossein Azami, Ryan Carlson, Courtney Comrie, Gabriela De La Cruz Sanchez, Chris Klimowski, Shuailong Li, Chuan Luo, Artin Majdi, Maliaca Oxnam, Travis Struck. That workshop was hosted by [the BIO5 Initiative][bio5], in partnership with [CyVerse][cyverse], [the D7 Data Science Institute][d7] and [the UArizona Libraries][uoa-libraries]
* Dr. Kimberly Meechan, David Palmquist, Prof. Ulf Schiller, and Dr. Robert Turner have taken over as Maintainers and core contributors for the lesson, and continue to drive its development.
* Many community members have opened issues and pull requests to improve the lesson.
* The lesson development process was supported by Dr. Erin Becker and Dr. Toby Hodges from The Carpentries Curriculum Team.


[alpha1]: https://tobyhodges.github.io/2020-01-14-heidelberg/
[alpha2]: https://ua-carpentries-workshops.github.io/2020-02-22-Tucson/
[AoE]: https://en.wikipedia.org/wiki/Anywhere_on_Earth
[application]: https://forms.gle/WFuG9tHivEPp2GvA9
[bio5]: https://bio5.org/
[call-for-contributors]: https://carpentries.topicbox.com/groups/discuss/Ta8ff359298db95c6-M390cec7393b29ed4b74bdda5/looking-for-contributors-maintainers-for-image-processing-with-python-lesson
[cyverse]: https://cyverse.org/
[dc-astro]: https://datacarpentry.org/astronomy-python/
[divas]: https://web.doane.edu/Colleges-Divisions-Programs/College-of-arts-sciences/Science-Mathematics-and-information-science-and-technology/Biology-Department/Divas-Project
[d7]: https://datascience.arizona.edu/
[embl]: https://embl.de/
[embl-bio-it]: https://bio-it.embl.de/
[jupyter]: https://jupyter.org/
[lesson]: https://datacarpentry.org/image-processing/
[opencv]: https://docs.opencv.org/4.5.5/
[prereq-list]: https://datacarpentry.org/image-processing/prereqs/index.html
[skimage]: https://scikit-image.org/
[uoa]: https://www.arizona.edu/
[uoa-libraries]: https://new.library.arizona.edu/
