---
layout: page
authors: ["Zhian N. Kamvar"]
teaser: "Working through chopportunities"
title: "The Dovetail #2: Updates from The Carpentries Workbench"
date: 2022-06-08
time: "09:00:00"
tags: ["Lesson Infrastructure", "Community", "Carpentries Workbench", "Beta", "Dovetail"]
---

This is the second post in a series that we are calling "The Dovetail."
In this series, we aim to keep members of The Carpentries community abreast of
the current news for [The Carpentries Workbench](https://carpentries.github.io/workbench). 

If you are interested in participating in discussions around The Carpentries
Workbench, head over to our GitHub Discussions forum: <https://github.com/carpentries/workbench/discussions>

## Updates to The Carpentries Workbench

Since 2022-05-25, 

 - [{sandpaper} version 0.5.5 -> 0.5.8](https://carpentries.github.io/sandpaper/news/index.html#sandpaper-058)
   - pull request workflow updated to include validation for lesson accessibility. 
     Links and images that could be improved for accessibility will now be
     highlighted in the pull request.

     <figure style="text-align: center">
       <img src="{{site.urlimg }}/blog/2022/06/2022-06-08-check-warnings.png" 
        alt="Screen capture of the 'files changed' tab of a pull request showing one line of text changed to include uninformative and missing links. Below the changed text are two alert boxes that show check warnings on that particular line of the file."/>
       <figcaption>
       GitHub will flag images with no alt text and links that are missing or have inaccessible descriptions.
       </figcaption>
     </figure>
 - [{varnish} version 0.1.13 -> 0.1.14](https://carpentries.github.io/varnish/news/index.html#varnish-0114)
   - Alerts for lesson development phase added
   - Lesson titles are now inline-block elements so long titles should wrap nicely
 - [{pegboard} version 0.2.6 -> 0.3.0](https://carpentries.github.io/pegboard/news/index.html#pegboard-030)
   - new method `$summary()` for lessons and episodes tabulates the different markdown elements.
   - Lessons can now analyze built files with the `$load_built()` method.
   - Bug fixes for showing `$error` and `$output` code blocks

To update your local Workbench installation, open R and use the following code:

```r
# Enable repository from carpentries
options(repos = c(
  ropensci = 'https://carpentries.r-universe.dev',
  CRAN = 'https://cloud.r-project.org'))
# Download and install sandpaper in R
install.packages(c('tinkr', 'pegboard', 'sandpaper', 'varnish'))
```

## Upcoming and Current Lessons in Workbench Beta

Schedule for the upcoming lessons coming soon! There are a few bottlenecks in
order to start beta testing for The Workbench:

1. We are still working on the correct workflow for uploading our lessons to AWS
   with the correct permissions so that we can dual deploy lessons for the
   stable and beta versions.
1. Our [lesson transition
   toolchain](https://github.com/data-lessons/lesson-transition#readme) is
   being modified to safely update lessons for entry into the workbench beta
   phase. It can enter lessons into pre-beta, but because [this transition is
   irreversible](https://github.com/data-lessons/lesson-transition#readme), great care must be taken.
1. We are working on [creating archives of our lessons](https://ropensci.org/blog/2022/03/22/safeguards-and-backups-for-github-organizations/)
   that can be included in the zenodo releases should they need to be reinstated.

We are working hard at resolving these bottlenecks so that we can commence with
the testing!

### New Participants

From our [original call for participants in the workbench beta phase]({{ site.url }}/blog/2022/05/workbench-beta/), we have gotten two new responses, for a total of seventeen community members officially participating in the beta phase:

 - **[Jon Haitz Legarreta Gorroño](https://github.com/jhlegarreta/), Lesson Developer (in The Carpentries Incubator)**
 - **[Karen Word](https://github.com/karenword/), Maintainer**
 - [Luis J. Villanueva](https://github.com/villanueval/), Maintainer
 - [Jon Wheeler](https://github.com/jonathanwheeler01/), Lesson Developer (in The Carpentries Incubator)
 - Simon Christ, Lesson Developer (in The Carpentries Incubator)
 - [Maneesha Sane](https://github.com/maneesha/), Instructor
 - [Sarah Brown](https://github.com/brownsarahm/), Maintainer
 - [Joel Nitta](https://github.com/joel.nitta/), Translator
 - [Juan Fung](https://github.com/juanfung/), Maintainer
 - [Jannetta Steyn](https://github.com/jsteyn/), Lesson Developer (in The Carpentries Incubator)
 - [Michael Joseph](https://github.com/josephmje/), Lesson Developer (in The Carpentries Incubator)
 - [Sarah Stevens](https://github.com/sstevens2/), Lesson Developer (in The Carpentries Incubator)
 - [Kozo Nishida](https://github.com/kozo2/), Lesson Translation (to Japanese)
 - François Michonneau, Maintainer
 - [Jamie Jamison](https://github.com/jmjamison/), Maintainer
 - Jennifer Stubbs (she/her), Instructor
 - [Drake Asberry](https://github.com/drakeasberry/), Maintainer

## Updates from Community About Working in Workbench Beta

None yet! Stay tuned!

## Tips and Tricks for Using The Workbench

The [syntax for alt text in Workbench lessons](https://carpentries.github.io/workbench/transition-guide.html#figures)
is a little different than the syntax you may be used to:

```markdown
![caption](image.png){alt='alt text'}
```

The reason for this is because the text inside of the square braces (`[]`) can actually be
rendered as markdown, so it makes more sense to use that as the figure caption, which can be formatted visually.
The alt text first and foremost is text that needs to be accessible, so
formatting is not as important.

Of course, your alt text is _rarely_ going to fit within a single line, so
instead of writing it as one long line, you can wrap the lines of text so that it
fits within the page. An example:

```markdown
![The author and his handsome son](fig/2022-06-08-author-cat.jpg){alt='A vertical
selfie photograph of Zhian (a Persian man) with thick-rimmed glasses and
short dark hair wearing headphones. His grey cat is sitting in his lap, looking
content as his head is being scratched.'}
```


<figure style="text-align: center">
  <img src="{{site.urlimg }}/blog/2022/06/2022-06-08-author-cat.jpg" width="50%"
   alt="A vertical selfie photograph of Zhian (a Persian man) with thick-rimmed glasses and short dark hair wearing headphones. His grey cat is sitting in his lap, looking content as his head is being scratched."/>
  <figcaption>
  The author and his handsome son
  </figcaption>
</figure>

You can find out more in [the figures section of the Workbench Documentation](https://carpentries.github.io/sandpaper-docs/episodes.html#figures).
