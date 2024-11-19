---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "A look back at styles"
title: "The Dovetail #16: Updates from The Carpentries Workbench"
date: 2023-03-14
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the sixteenth post in [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail) (our new lesson infrastructure).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 
If you are unfamiliar with The Workbench, you can [watch a video that describes
the workbench and the beta phase in two minutes](https://youtu.be/x7tETGpF3-4).

If you are interested in participating in discussions around The Carpentries
Workbench, or if you have questions, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

---

## Beta Phase to Complete on 03 April, 2023

We are nearing the end of the beta phase, which means that the lessons below will soon switch to The Workbench view as the default.
In April, be on the lookout for community discussions about The Workbench where you can get an introduction about what to expect when we transition all of our lessons in May. 

## Lessons Currently In the Beta Phase

The table below shows the status of lessons that are currently in the beta phase. 
All of these lessons are now in the [second (beta) stage](https://carpentries.github.io/workbench/beta-phase.html#beta) 
of the beta phase (one repository, two lesson websites).

| Lesson                                                   | Workbench URL                                                |
| -------------------------------------------------------- | ------------------------------------------------------------ |
| R for Social Scientists                                  | <https://preview.carpentries.org/r-socialsci>                |
| Introduction to Geospatial Raster and Vector Data with R | <https://preview.carpentries.org/r-raster-vector-geospatial> |
| Instructor Training                                      | <https://preview.carpentries.org/instructor-training>        |
| Análisis y visualización de datos usando Python          | <https://preview.carpentries.org/python-ecology-lesson-es>   |

[^1]: The Workbench beta phase is divided into three distinct stages, read more at <https://carpentries.github.io/workbench/beta-phase.html>.

## Thank You, Lesson Template Contributors

The Carpentries Workbench will become the default platform for maintaining official Carpentries lessons in May 2023, replacing [`carpentries/styles` (aka the "Lesson Template"](https://github.com/carpentries/styles)). 
As I have described in previous blog posts ([on design principles](https://carpentries.org/blog/2020/08/lesson-template-design/#pain-points-with-the-current-template) and [the (former) Lesson Infrastructure Committee](https://carpentries.org/blog/2020/08/lesson-template-design/#pain-points-with-the-current-template)), the lesson infrastructure already had come a long way by the time I joined in 2020 as a result of years of volunteer effort by [the Contributors to the template](https://github.com/carpentries/styles/graphs/contributors).

It is hard to overstate the impact of `carpentries/styles`. 
This "Lesson Template" has served as the foundation for _all_ of our lessons (which includes our > 60 official lessons, > 100 incubator lessons, workshop websites (yes, `carpentries/styles` is also the source for `carpentries/workshop-template`), AND the wider community who have adopted it for their own lessons and documentation.

You might notice that I place "Lesson Template" in quotes above.
This is because `carpentries/styles` is an _infrastructure_, not a template.
A template is something more akin to scaffolding to get you started and then discarded.
Lessons created with `carpentries/styles`, however have all the tools and styling resources embedded... tools and styling that need to be updated within the ever changing environment of web publishing.
This is where the Contributors and Maintainers of `carpentries/styles` come in. 

If you would pardon me a moment to make a small analogy: our lessons are a bit like a book of songs for piano[^2].
Anyone trained to play (i.e. certified Carpentries Instructors) can pick up the book and play the collection with little effort.
Lesson Developers and Maintainers are the composers, and the lesson infrastructure---is the piano.
But of course, pianos require regular tuning and maintenance and not everyone who can play a piano is skilled at tuning a piano.
Thus, if the lesson infrastructure is the piano, then the people who maintain and contribute to the lesson infrastructure are the piano tuners, without whom all pianos would eventually drift into dissonance.
Without the Contributors to our lesson infrastructure, the foundation for our lessons would have crumbled long ago.

[^2]: Assume popular songs (e.g. not [prepared piano](https://en.wikipedia.org/wiki/Prepared_piano) pieces)

When `carpentries/styles` was created, The Carpentries had a handful of lessons available and thus, it was not infeasible for one person to manually apply changes from the infrastructure to all the lessons in 20 minutes.
As the number of lessons grew, this became more and more of a burden.
It was akin to having one piano tuning company serve an entire metropolitan area: the expertise existed, but there was no capacity to meet demand.
The Workbench fixes this demand problem by separating out the tools from the template.
It is important to recognise that the progress made by The Workbench was built from the sucessess and lessons learned from development of `carpentries/styles`.

Thus, I would like to extend a thank you to all of [the Contributors to `carpentries/styles`](https://github.com/carpentries/styles/graphs/contributors).
In particular, I would like to highlight a few names who have been deeply involved in the project (in no particular order): Maxim Belkin, Kate Hertweck, Raniere Silva, Sarah M. Brown, François Michonneau, Renato Alves, Katrin Leinweber, Rémi Emonet, and Naupaka Zimmerman. 
Each one of these community members has consistently provided valuable discussions and improvements to the lesson infrastructure, from accessibility changes to the CSS to updates to the Makefile workflow to template language. 
But really, what makes or breaks an open source project like this is the participation from the community and `carpentries/styles` has never lacked that.
To all the contributors, I would like to say one thing before we transition to The Workbench; without the foundation of work you have laid, The Workbench would not be what it is today: and infrastructure that provides lesson developers a means to create accessible lessons that align with The Carpentries core values and teaching principles.

## Updates to The Carpentries Workbench

Since 2023-02-14, 

 - [{sandpaper} version 0.11.5 -> 0.11.8](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-0118)
   - Packages from BioConductor can now be bootstrapped in new lessons.
   - The package {renv} updated to 0.17.0, which [introduced many new bugs](https://github.com/carpentries/sandpaper/issues/406),
     It is recommended to avoid updating {renv} until its next release is sent to CRAN.
     If you have already updated, please visit [sandpaper issue 406](https://github.com/carpentries/sandpaper/issues/406) for details. 
 - [{pegboard} version 0.4.3](https://carpentries.github.io/pegboard/news/index.html#pegboard-043)
   - No updates :)
 - [{varnish} version 0.2.14](https://carpentries.github.io/varnish/news/index.html#varnish-0214)
   - No updates :)

To update your local Workbench installation, open R and use the following code:

```r
# Enable repository from carpentries
options(repos = c(
  ropensci = 'https://carpentries.r-universe.dev',
  CRAN = 'https://cloud.r-project.org'))
# Download and install sandpaper in R
install.packages(c('tinkr', 'pegboard', 'sandpaper', 'varnish'))
```

## Tips and Tricks for Using The Workbench

If you are working on a lesson and wish to make sure your links and images are
accessible, you can check the output of `sandpaper::validate_lesson()`, which
also runs every time you build your lesson. It will provide informative links
on forming accessible content: 

### Types of accessibility checks

From [the {pegboard} link validator documentation](https://carpentries.github.io/pegboard/reference/validate_links.html#accessibility-a-y-):

> Accessibillity ensures that your links are accurate and descriptive for people who have slow connections or use screen reader technology.
> 
> #### Alt-text (for images)
> 
> All images must have associated alt-text. In pandoc, this is acheived by writing the alt attribute in curly braces after the image: ![image caption](link){alt='alt text'}: <https://webaim.org/techniques/alttext/>
> 
> #### Descriptive text
> 
> All links must have descriptive text associated with them, which is beneficial for screen readers scanning the links on a page to not have a list full of "link", "link", "link": <https://webaim.org/techniques/hypertext/link_text#uninformative>
> 
> #### Text length
> 
> Link text length must be greater than 1: <https://webaim.org/techniques/hypertext/link_text#link_length>

### Example

File: `episodes/example.md`

```markdown 
---
title: 'Example Episode'
teaching: 1
exercises: 1
---

The Workbench ([click here](https://carpentries.org)) uses 
[R](https://r-project.org) and [pandoc](https://pandoc.org) to
build websites. 
```

The above example would produce the following output, telling you there are errors in two of the three links:

```
! There were errors in 2/3 links
◌ Avoid uninformative link phrases
<https://webaim.org/techniques/hypertext/link_text#uninformative>
◌ Avoid single-letter or missing link text
<https://webaim.org/techniques/hypertext/link_text#link_length>

episodes/example.md:7 [uninformative link text] 'click here'
episodes/example.md:8 [link text too short] 'R'
```

You could then go back to your file and correct those accessibility issues:


```markdown 
---
title: 'Example Episode'
teaching: 1
exercises: 1
---

[The Workbench](https://carpentries.org) uses 
[the R programming language](https://r-project.org) and 
[pandoc](https://pandoc.org) to build websites. 
```

