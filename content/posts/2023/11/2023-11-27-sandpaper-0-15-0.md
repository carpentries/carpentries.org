---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Updates to instructor view, doi badges, and more"
title: "Release of Sandpaper 0.15.0"
date: 2023-11-27
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the eighteenth post continuing [a series that we are calling "The Dovetail",
about the transition to The Carpentries Workbench](https://carpentries.org/posts-by-tags/#blog-tag-dovetail) (our new lesson infrastructure).
In this series, we aim to keep members of The Carpentries community abreast of
the current news about [the Workbench](https://carpentries.github.io/workbench). 
If you are unfamiliar with The Workbench, you can [watch a video that describes
the workbench and the beta phase in two minutes](https://youtu.be/x7tETGpF3-4).

If you are interested in participating in discussions around The Carpentries
Workbench, or if you have questions, head over to our [GitHub Discussions forum](https://github.com/carpentries/workbench/discussions).

<span style='font-size: large;'>If you have used the workbench and would like to provide feedback, please
<b><a href='https://carpentries.typeform.com/to/KRBl4IZM'>tell us about your experience</a>.</b></span> 

## Six months of success

As of 16 November 2023, we acheived a milestone of 6 months where all of our lessons
have been using The Workbench. Since the last update on 13 April 2023, we have
seen a huge outpouring of support from the community to support the lesson
transition phase that was finalized on 16 May 2023 when [Foundations of
Astronomical Data Science](https://datacarpentry.org/astronomy-python/) was
transitioned to use The Workbench. 

Since then, we have been hard at work to shore up capacity within the Core Team
while fixing bugs and implementing new features such as the processing of
workshop overview pages, child documents, and a `spoiler` class of fenced divs
to collapse parts of the lesson. 

## Sandpaper 0.15.0 to be released on 29 November 2023

In this next version of the user interface to The Workbench, we have
implemented features that have been requested. 

1. R Markdown lessons can choose to render a handout by using `handout: true`
   in their `config.yaml` (this will be available for all lessons with the
   release of pegboard 0.8.0). 
2. The "More" dropdown menu for the Instructor view will now also contain links
   to the learner materials underneath the Instructor materials.    
   ![screenshot of a dropdown menu from "intstructor training" that is split
   into two sections: one section for instructors and another with links for
   learners]({{ site.urlimg }}/blog/2023/11/2023-11-22-instructor-screen.png)
3. For peer-reviewed lessons, adding a `doi:` with a valid DOI in the
   `config.yaml` will have a DOI badge to appear in the tool bar that links to
   the publication or archive (see image below).
4. For those building the lessons in Docker, the `site/` folder is now
   customisable using the `SANDPAPER_SITE` environment variable.

In addition, we will release {varnish} 0.4.0, which will update the visual
styling of the status badges to make them more prominent.

<figure>
  <img src='{{ site.urlimg }}/blog/2023/11/2023-11-10-doi-screen.png' alt='carpentries logo with a pale yellow badge with a blue border that says "DOI" with a doi number appended' style='border: solid 1pt black;'/>
  <img src='{{ site.urlimg }}/blog/2023/11/2023-11-10-beta-screen.png' alt='carpentries logo with a blue badge that says "beta"' style='border: solid 1pt black;'/>
  <img src='{{ site.urlimg }}/blog/2023/11/2023-11-10-alpha-screen.png' alt='carpentries logo with a yellow badge that says "alpha"' style='border: solid 1pt black;'/>
  <img src='{{ site.urlimg }}/blog/2023/11/2023-11-10-pre-alpha-screen.png' alt='carpentries logo with a red badge that says "pre-alpha"' style='border: solid 1pt black;'/>
  <figcaption>
  The new badge formats. 
  </figcaption>
</figure>

All this along with documentation upgrades and bugfixes will be available
starting on 29 November 2023, and it will automatically propogate to all lessons by
5 December 2023.

## Giving Thanks

It has been over six months since we wrote a Dovetail blog post and needless to
say, there are a lot of people that I would like to thank. I'm grateful for
everyone who has taken the opportunity to open issues in The Workbench
repositories to report bugs or features needed. I'm especially grateful for
everyone who has additionally opened pull requests to fix these bugs. 

The whole reason this project works is because of the community. Full stop.
Below, I list all the contributors from GitHub who have opened issues or pull
requests that have lead to bugfixes or features in The Workbench, but I do want
to acknowledge that there are so many more people who could be named here,
including the Maintainers who have been able to give feedback directly in
Maintainer meetings, Lesson Developers working in The Carpentries Incubator
giving feedback about their use case, everyone from the internationalisation
community whose continued efforts bring us closer to natively supporting
translations, and last but not least, the brave souls who are willing to open
an issue and dream that we will continue to grow.

### Sandpaper

Thank you to all the people who have who have contributed to or opened issues
that have led to the improvement of {sandpaper} since version 0.11.15:
[@froggleston](https://github.com/froggleston),
[@karenword](https://github.com/karenword),
[@ErinBecker](https://github.com/ErinBecker),
[@fherreazcue](https://github.com/fherreazcue),
[@tobyhodges](https://github.com/tobyhodges),
[@milanmlft](https://github.com/milanmlft),
[@apirogov](https://github.com/apirogov),
[@fnattino](https://github.com/fnattino),
[@tesaunders](https://github.com/tesaunders),
[@mwhamgenomics](https://github.com/mwhamgenomics),
[@kaijagahm](https://github.com/kaijagahm),
[@jcolomb](https://github.com/jcolomb),
[@klbarnes20](https://github.com/klbarnes20),
[@ocaisa](https://github.com/ocaisa),
[@joelnitta](https://github.com/joelnitta),
[@velait](https://github.com/velait),
[@cynthiaftw](https://github.com/cynthiaftw),
[@debpaul](https://github.com/debpaul),
[@bencomp](https://github.com/bencomp),
[@ostephens](https://github.com/ostephens)
and [@twrightsman](https://github.com/twrightsman)

### Pegboard

Thank you to all the people who have who have contributed to or opened issues
that have led to the improvement of {pegboard} since version 0.5.2:
[@joelnitta](https://github.com/joelnitta),
[@trhallam](https://github.com/trhallam),
[@tobyhodges](https://github.com/tobyhodges),
[@klbarnes20](https://github.com/klbarnes20),
[@beastyblacksmith](https://github.com/beastyblacksmith),
[@ErinBecker](https://github.com/ErinBecker)
and [@uschille](https://github.com/uschille)

### Varnish

Thank you to all the people who have contributed to or opened issues
that have led to the improvement of {varnish} since version 0.2.16:
[@brownsarahm](https://github.com/brownsarahm),
[@froggleston](https://github.com/froggleston),
[@tobyhodges](https://github.com/tobyhodges),
[@Robadob](https://github.com/Robadob),
[@marklcrowe](https://github.com/marklcrowe)
and [@bencomp](https://github.com/bencomp)



