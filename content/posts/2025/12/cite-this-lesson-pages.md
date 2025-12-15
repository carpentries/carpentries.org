---  
layout: page  
authors: ["Toby Hodges", "Robert Davey", "Erin Becker"]  
teaser: "The new release of the lesson infrastructure also includes Mermaid diagram support and several other new features"  
title: "Introducing Cite This Lesson Pages to The Carpentries Workbench"  
date: 2025-12-17  
time: "09:00:00"  
tags: ["Curriculum", "Carpentries Workbench", "Internationalisation", "Publishing"]  
---

A new version of The Carpentries Workbench was released this month, and included several exciting new features.

## *Cite This Lesson* Pages

[*Cite This Lesson* pages](https://carpentries.github.io/lesson-development-training/citation.html) will now be included in any lesson with a `CITATION.cff` file in the source repository. By displaying contributor information as a part of the lesson website, these pages will provide a lot more visibility to all the people who have made the lesson what it is. The Curriculum Team has been hoping to provide this kind of acknowledgement to lesson contributors for many years, and this is a major step towards the establishment of a regular release cycle for Carpentries lessons.

![Screenshot of the Acknowledgements and Citations section of a lesson, with a Cite This Lesson page.](/blog/2025/12/cite-this-lesson.png)

Maintainers of Data Carpentry, Library Carpentry, and Software Carpentry lessons will receive support from the Curriculum Team to populate a `CITATION.cff` in their lesson repository during the first months of 2026\. Community members using the Workbench to develop and maintain their own lessons (in the Incubator and elsewhere) can refer to the [documented recommendations for the contents of the citation file](https://carpentries.github.io/sandpaper-docs/editing.html#making-your-lesson-citable) when creating their own `CITATION.cff`.

If you teach a lesson or adapt it for your own projects, please cite the lesson (and [the Workbench itself](https://carpentries.org/workbench/#cite-the-workbench)) in any written reports, publications, etc. you make.

## Mermaid Diagram Support

The latest release also includes support for [Mermaid.js diagrams](https://mermaid.js.org/), a feature contributed to the Workbench by [Dimitrios Theodorakis](https://github.com/astroDimitrios). Thanks, Dimitrios! Mermaid provides a framework for describing diagrams of various types in the source Markdown of a lesson. The figures are then rendered in the lesson webpages by the Mermaid JavaScript library. [Visit the University of Sheffield’s *Git With it* lesson](https://fair2-for-research-software.github.io/git-with-it/branching.html#branches) for an example of one type of Mermaid diagram: the GitGraph.

## Linking to Language Variants of a Lesson

Another feature, contributed by [Renato Alves](https://github.com/unode), provides a way for lesson maintainers to [link out to versions of that lesson available in other languages](https://carpentries.github.io/sandpaper-docs/editing.html#offering-4-languages-english-spanish-german-and-italian). This will be immediately helpful to some community members who have produced translated/localised versions of lessons already. 

It also represents an important step to supporting the ongoing internationalisation efforts of the Carpentries community, taking place [on CrowdIn](https://carpentries.crowdin.com/). Watch this space for more progress on that front: documentation about internationalisation is planned for [the community handbook](https://docs.carpentries.org/) in 2026, and the Core Team hopes to be able to support closer integration/alignment of these community efforts with official lesson maintenance soon too. In the meantime, community members interested in getting involved in the localisation of lessons should join the `#internationalisation` channel on Slack.

## Coming Soon: Improved Lesson Build/Maintenance Workflows

Finally, although not in this release, major improvements are coming to the workflows that build and maintain lessons on GitHub in January. We had hoped to roll them out already but need a little more time to test everything out and make sure that the upgrade will not be disruptive.

The improvements will be worth the wait: they will bring major improvements to the stability of the infrastructure through the use of containers, and reduce the time it takes to build and deploy lessons when changes are made to the content. The availability of maintained containers for the Workbench will also provide an easy way for community members to install the infrastructure on their local system.