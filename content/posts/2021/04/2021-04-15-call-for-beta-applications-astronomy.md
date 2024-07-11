---
layout: page
authors: ["Rodolfo Montez Jr.", "Azalee Bostroem", "Erin Becker"]
teaser: "Apply to host or teach a beta pilot workshop for the newest Data Carpentry curriculum"
title: "Foundations of Astronomical Data Science - Call for Beta Pilot Applications"
date: 2021-04-15
time: "09:00:00"
tags: ["Curriculum", "Pilot Workshops"]
---

The [Astronomy Data Carpentry curriculum](https://datacarpentry.org/astronomy-python/), “Foundations of Astronomical Data Science”  successfully held two alpha workshops in November 2020 and January 2021.

We are seeking community members to host and teach [beta pilot workshops](https://cdh.carpentries.org/the-lesson-life-cycle.html#overview-and-definitions) with the revised [Foundations of Astronomical Data Science](https://datacarpentry.org/astronomy-python/) curriculum in June - August 2021. Continue reading for more information on the lessons, the alpha workshops, and to apply to host a beta pilot workshop.

The Astronomy Data Carpentry project is an endeavor funded by the American Institute of Physics [Venture Partnership Fund](https://www.aip.org/aip/member-benefits/venture-partnership-fund/winners), which was awarded to the American Astronomical Society to develop this curriculum (PIs: Azalee Bostroem, Diane Frendak, and Dr. Rodolfo Montez Jr.). The Astronomy Curriculum Development Committee, composed of Azalee Bostroem (Project Lead; University of California, Davis), Dr. Erin Becker (The Carpentries Associate Director), Dr. Rodolfo Montez Jr. (Astronomy Advisor; AAS and AIP liaison), Dr. Brett Morris (Astronomy Advisor), and Dr. Phil Rosenfield (Astronomy and Industry Advisor), were joined by lead curriculum developer, Dr. Allen Downey (Olin College), to create a two-day Data Carpentry curriculum for the astronomical community.

## About the Astronomy Data Carpentry Curriculum

The [Foundations of Astronomical Data Science](https://datacarpentry.org/astronomy-python/) curriculum covers a range of core concepts aimed at efficient study of the growing datasets facing the astronomical community. In particular, the curriculum teaches learners to work with astronomy-specific packages (Astropy, Astroquery) and more general packages (Pandas) to perform database operations (SQL queries, joins, filtering) to create publication-quality data visualisations. These concepts are demonstrated on the large, all-sky, multi-dimensional dataset from the [Gaia satellite](https://sci.esa.int/web/gaia), which measures the positions, motions, and distances of approximately a billion stars in our Milky Way galaxy with unprecedented accuracy and precision, and the [Pan-STARRS](https://panstarrs.stsci.edu/) photometric survey, which precisely measures light output and distribution from many stars. Together, these datasets are used to reproduce part of the analysis from the article [“Off the beaten path: Gaia reveals GD-1 stars outside of the main stream”](https://arxiv.org/abs/1805.00425) by Drs. Adrian M. Price-Whelan and Ana Bonaca. The lessons show how to identify and visualize the GD-1 stellar stream, which is a globular cluster that has been tidally stretched by the Milky Way.

![Stellar streams identified in the Gaia survey.](https://www.cosmos.esa.int/documents/29201/239681/IoW_20190418Update_MW_Stream_Map_small.jpg/a4fac38f-c0b4-2a6f-596c-5722ec7bbe86?t=1555593319529)

Stellar streams identified in the Gaia survey. Credits: ESA/Gaia/DPAC, Khyati Malhan from the Observatoire Astronomique de Strasbourg, Rodrigo A. Ibata from CNRS, Nicolas F. Martin from CNRS

## Alpha Pilot Workshops

The first pilot workshop was held over five half days in November 2020, and reached 21 participants. Over the five days of the workshop (held virtually due to the pandemic), lead instructors (Downey and Bostroem) delivered the material via Zoom while a rotation of helpers fielded technical challenges and questions via the accompanying Slack channel. The workshop ran for 4 hours each day.

Our second alpha pilot was also the first public workshop using this curriculum - offered at the virtual winter meeting of the American Astronomical Society over two days (7-8 January 2021). 35 registered students, 3 instructors (Downey, Montez, Bostroem), and 3 helpers met for 7 hours a day on Zoom and Slack. Improvements from the pilot session helped streamline the curriculum for this more condensed format.

We are extremely grateful to all the pilot alpha learners for being enthusiastic learners and providing detailed feedback throughout the workshop by asking questions, openly troubleshooting, and completing the minute-card assessments and daily surveys. We owe the learners a great deal for helping advance and improve the curriculum to its current state.
Special thanks is due to our workshop helpers Drs. Iva Momcheva (Space Telescope Science Institute), Meredith Rawls (University of Washington), Phil Rosenfield, Rodolfo Montez Jr, and Erin Becker for answering many questions, troubleshooting, and supporting learners throughout the two alpha pilots.

### What Went Well
- Learners unanimously agreed that the workshop taught skills that are currently important or will be important for astronomers to know in the next 5+ years and would recommend this workshop to a colleague at their level of programming experience.

- A majority of learners gained confidence in the following key skills from the lessons: writing database queries, performing database join operations, using Astropy Tables, Panda DataFrames, FITS and HDF5 files, and Astropy coordinates and units.

![Pie chart showing all 33 learners agreed the workshop taught skills important for astronomers to know.]({{ site.urlimg }}/blog/2021/04/acdc_510years.png)

### What We Have Revised

- During the first pilot, we ran into a major cross-platform problem with the interactive matplotlib function `ginput`. Originally, we were using `ginput` to allow for user input for source selections by defining a closed polygon region. In the first pilot we temporarily remedied the widespread error by distributing polygon coordinates via the Slack channel. By the second pilot, we abandoned `ginput` for a scientific approach using an isochrone model.

- This curriculum relies on uninterrupted connectivity with the Gaia database servers. In both alpha workshops we encountered users being temporarily locked out of the Gaia database servers during the part of the lesson that uploads a file to be used as part of a query. We have revised the lessons to avoid uploading a file, opting instead for building onto previously built queries.

- Many of the lessons now end with the learner storing lesson data to a file. If a user later encounters an error or is unable to execute a query, this file can be accessed to continue the lesson. During the alpha workshops, we provided these files for download as needed. For the beta workshops, the learners will download the files as part of the setup instructions.

- During the two alpha workshops, we relied on copying and pasting code from earlier lessons to use in later lessons; typically, we used these code snippets to create functions. For the beta workshops, these functions are better integrated into the lesson material and the function library is also distributed as part of the setup instructions.

## Apply to Host a Beta Pilot Workshop

We are reaching out to the community for volunteers to host beta pilot workshops of the [Foundations of Astronomical Data Science](https://datacarpentry.org/astronomy-python/) curriculum.  Beta pilots are an important step in the process of developing a new lesson, as these represent the moment when material is taught for the first time by someone other than the original authors.

Beta pilot instructors should:
- Be certified Carpentries Instructors and have taught at least 2 Carpentries workshops.
- Have experience working with astronomical data and common astronomical file formats.

Beta pilot Instructors commit to:
- Participating in 1-2 hours of onboarding led by lesson developers prior to their workshop. Every effort will be made to offer this onboarding asynchronously as well as synchronously.
- Teaching the material over 2 full days of instruction (~10-12 hours instructional time) in June - August 2021 (exact dates to be determined).
- Advertising to and recruiting appropriate learners. Learners for this workshop should have at least an undergraduate level background in astronomy, and already have experience with bash shell and Python programming equivalent to that taught in a Software Carpentry Python workshop.
- Providing feedback to the lesson developer(s) after their workshop to enable the lesson to be further polished in final preparation for an official release.

If you would like to host a pilot of the lesson at your institute/organisation, please take a few minutes to [fill out this short application form](https://forms.gle/5sK9DKvptHBBUqTw9) before the end of Friday 30 April 2021 ([anywhere on Earth](https://en.wikipedia.org/wiki/Anywhere_on_Earth)). The information collected there will help us coordinate the pilot process and maximise the impact of the process on the lesson material.

If you have any questions about lesson development and the beta pilot process, please contact [Erin Becker](mailto:ebecker@carpentries.org). For more information about the lesson itself, please contact [Azalee Boestroem](mailto:abostroem@gmail.com).
