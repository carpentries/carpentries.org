---
title: Curricula Overview
layout: single
---

## Data Carpentry: Astronomy
This [workshop][dc-astro] covers a range of core concepts necessary to
efficiently study the ever-growing datasets developed in modern astronomy.
In particular,
this curriculum teaches learners to perform database operations (SQL queries, joins, filtering) and
to create publication-quality data visualisations.
The workshop uses two large astronomical datasets: data from the Gaia sattelite and the Pan-STARRS prohotmetric survey.
Data Carpentry: Astronomy has more prerequisites than most of our workshops,
requiring learners to have some familiarity with astronomical concepts
and the Python programming language.

## Data Carpentry: Ecology
This [workshop][dc-ecology] covers data organisation with spreadsheets, data cleaning with OpenRefine, and some data analysis and plotting (with your
choice of R or Python). This workshop is intended for anyone working with tabular data (data with rows and columns, e.g. Excel). The data
used for this workshop is an ecology dataset - counts of animal species that were observed in different locations over time, along with
information about their sex, weight, etc. This data is easily understandable by non-ecologists and is considered our most general-purpose
workshop.

## Data Carpentry: Genomics
This [workshop][dc-genomics] is intended for people working with high-throughput sequencing data and focuses on helping them upgrade their workflow from
relying on spreadsheets and GUI platforms to using command-line tools and remote computing power. This workshop is taught using Amazon
Web Services. Learners will be introduced to core Bash commands and will learn to write custom Bash scripts to automate an analysis
pipeline. They will be introduced to some commonly used command-line bioinformatics tools and file formats. This workshop does not cover
individual methods for working with RNA-seq, ChIP-seq, or other specialized datasets, but instead focuses on core principles for
efficient and reproducible research with sequencing data.

## Data Carpentry: Geospatial
This [workshop][dc-geospatial] is intended for people working with geospatial data (i.e. data that can be plotted on a map). It starts out with a short
introduction to essential geospatial concepts and a shortened version of our core R lesson before progressing into working with
specialized geospatial packages in R. This workshop gets learners to a fairly advanced stage of creating geospatial plots (i.e. maps of
data distributions), but does not cover data organisation or cleaning. For a more general workshop covering these topics, please check
out our [Ecology](#data-carpentry-ecology) and [Social Sciences](#data-carpentry-social-sciences) curricula.

## Data Carpentry: Image Processing
This [workshop][dc-image] teaches the concepts and skills needed to
write automated processing pipelines for image data.
Using examples from morphometrics, the curriculum covers
the steps of a typical image processing workflow:
loading images, masking, blurring and thresholding data,
and ends with a capstone challenge to provide a chance for additional practice.
The workshop uses a variety of example images that do not require any domain-specific knowledge.
However, the curriculum does require learners to have gained some familiarity with
the Python programming language,
such as by attending a [Software Carpentry](#software-carpentry-plotting-and-programming-in-python),
[Data Carpentry: Ecology](#data-carpentry-ecology) or
[Data Carpentry: Social Sciences](#data-carpentry-social-sciences) workshop.

## Data Carpentry: Social Sciences
This [workshop][dc-socialsci] covers data organisation with spreadsheets, data cleaning with OpenRefine, and some data analysis and plotting with R. This
workshop is very similar to our [Ecology](#data-carpentry-ecology) workshop, but uses a dataset more relevant for social scientists, particularly those working with
interview data. The data used for this workshop is a set of interview responses from interviews of farmers in two countries in eastern
Africa about their agricultural practices and household resources. This workshop uses restricted-response data and does not cover
qualitative data analysis or analysis of free-text responses.

## Library Carpentry
This [workshop][lc] is intended for people working in libraries and the information sciences. It introduces terms, phrases, and concepts in
software development and data science, how to best work with data structures, and use regular expressions in searches. We introduce the
Unix-style command line interface, and teach basic shell navigation, as well as the use of loops and pipes for linking shell commands.
We also introduce grep for searching and subsetting data across files. Exercises cover the counting and mining of data. In addition, we
cover working with OpenRefine to transform and clean data, and the benefits of working collaboratively via Git/GitHub and using version
control to track your work.

## Software Carpentry (All Workshops)
All [Software Carpentry][swc-all] workshops include an introduction to Bash shell scripting and version control with Git, along with your choice of
either R or Python. Learners will gain confidence in using the command-line to navigate their file structure and work with files on their
computer, culminating in writing custom Bash scripts to automate repetitive analyses. They will learn the core concepts of version
control and be able to implement a simple Git workflow for tracking their own work. Software Carpentry workshops also include your
choice of one of our R or Python lessons (listed below).

## Software Carpentry (Plotting and Programming in Python)
Our more introductory Python lesson. In addition to our standard content, this workshop covers data analysis and
visualisation in Python, focusing on working with core data structures (including tabular data, not covered in our Programming with
Python lesson), using conditionals and loops, writing custom functions, and creating customised plots. As our more introductory Python
offering, this workshop also introduces learners to JupyterLab and strategies for getting help. This workshop is appropriate for learners
with no previous programming experience. For audiences with some experience with Python or other programming languages, we recommend our
[Programming with Python](#software-carpentry-programming-with-python) lesson.

## Software Carpentry (Programming with Python)
Our more advanced Python lesson. In addition to our standard content, this workshop covers data analysis and
visualisation in Python, focusing on working with core data structures, using conditionals and loops, writing custom functions, and
running Python programs from the command line. This is the more advanced of our two Python offerings for Software Carpentry and is
appropriate for learners with some previous programming experience, in Python or other languages. For audiences with no previous
programming experience, we recommend our [Plotting and Programming in Python](#software-carpentry-plotting-and-programming-in-python) lesson.

## Software Carpentry (R for Reproducible Scientific Analysis)
Our more introductory R lesson. In addition to our standard content, this workshop covers data analysis and
visualisation in R, focusing on working with tabular data and other core data structures, using conditionals and loops, writing custom
functions, and creating publication-quality graphics. As our more introductory R offering, this workshop also introduces learners to
RStudio and strategies for getting help. This workshop is appropriate for learners with no previous programming experience. For audiences
with some experience with R or other programming languages, we recommend our [Programming with R](#software-carpentry-programming-with-r) lesson.

## Software Carpentry (Programming with R)
Our more advanced R lesson. In addition to our standard content, this workshop covers data analysis and
visualisation in R focusing on working with core data structures, using conditionals and loops, writing custom functions, and running R
programs from the command line. This is the more advanced of our two R offerings for Software Carpentry and is appropriate for learners
with some previous programming experience, in R or other languages. For audiences with no previous programming experience, we recommend
our [R for Reproducible Scientific Analysis](#software-carpentry-r-for-reproducible-scientific-analysis) lesson.

## Community Developed Lessons
In addition to the established curricula listed above,
many members of our community work to develop new lesson material
on a wide range of topics.
You can see a list of these lessons on our
[Community Developed Lessons page][community-lessons].
We hope you find a lesson there that suits your needs and interests.
These materials exist at varying stages of maturity,
from only the basics of a lesson outline up to and
including stable lessons with a full set of exercises and solutions,
and The Carpentries accepts no responsibility for
their accuracy or quality.
The content of most community developed lessons is liable to change at any time.
Your perspective is a valuable resource to help improve all our lessons!
If you do learn or teach from any lesson under community development,
please take the time to provide feedback on your experience to the authors.

[community-lessons]: /community-lessons/
[dc-astro]: https://datacarpentry.org/lessons/#astronomy
[dc-ecology]: https://datacarpentry.org/lessons/#ecology
[dc-genomics]: https://datacarpentry.org/lessons/#genomics
[dc-geospatial]: https://datacarpentry.org/lessons/#geospatial
[dc-image]: https://datacarpentry.org/lessons/#image-processing
[dc-socialsci]: https://datacarpentry.org/lessons/#social-science
[lc]: https://librarycarpentry.org/lessons/
[swc-all]: https://software-carpentry.org/lessons/
