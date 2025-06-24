---
layout: page
authors: ["John Chodacki", "Steve Diggs", " Erin Becker", "Kari L. Jordan", "Emily Katz"]
teaser: "Learn about the important steps taken toward co-creating new lesson content!"
title: "Building Skills with Generalist Repositories: An Update on the Carpentries + GREI Collaboration"
date: 2025-06-26
time: "18:00:00"
tags: ["Curriculum", "Community"]
---

In late 2024, we launched a collaboration between The Carpentries and the [Generalist Repository Ecosystem Initiative (GREI)](https://datascience.nih.gov/data-ecosystem/generalist-repository-ecosystem-initiative), aiming to explore how generalist data repositories such as [Dataverse](https://dataverse.harvard.edu/), [Dryad](https://datadryad.org/), [Figshare](https://figshare.com/), [Mendeley Data](https://data.mendeley.com/), [Open Science Framework](https://osf.io/), [Vivli](https://vivli.org/), and [Zenodo](https://zenodo.org/) might be more intentionally woven into the data skills we teach. Since then, we've taken important steps toward that vision by co-creating new lesson content, running an in-person workshop, and inviting the community into a broader conversation about data sharing and discoverability.

But just as important as the actions we took were the questions we asked: What would it look like if open data repositories weren’t just add-ons at the end of a workflow, but upfront teaching concepts in our lessons? How can we position generalist repositories as active components in retrieving and processing datasets? How can we give researchers the tools not just to write clean code, but to publish their work in ways that make it reusable and citable by others?

## From Skills to Sharing: Connecting the Workflow

Researchers should be able to share any dataset, even those that don't fit neatly into a disciplinary home, and doing so should be simple, supported, and aligned with [FAIR principles](https://www.go-fair.org/fair-principles/). Additionally, researchers should be able to leverage data sets directly from repositories as they do their analysis. But these ideas only work if researchers know these tools exist and understand how to use them.

To explore this further, we deposited our lesson datasets into a generalist repository (in this case, [Zenodo](https://zenodo.org/)), assigning them DOIs to make them citable and persistently accessible. This wasn’t just about modelling good archival practice; it was about rethinking how researchers interact with data during analysis. By modifying the lessons to retrieve datasets programmatically via API, we removed the need to download files locally and gave learners a real-world example of how generalist repositories can support active, iterative research workflows. It’s a shift in perspective—from repositories as endpoints for finished work to resources that support reproducible, reusable, and automated analysis.

Then, in our [Python Gapminder lesson](https://swcarpentry.github.io/python-novice-gapminder/), we adjusted the lesson to showcase this. Traditionally, we teach students how to load a local CSV file from the local filesystem using pandas. In the GREI-enhanced version of the lesson, we added a new challenge: what if that file came from a repository like Zenodo? What if learners could use a DOI to fetch data directly via an API and cite it properly in their research? These kinds of integrations change the framing—from “how do I analyse this file?” to “how do I responsibly work with, and contribute back to, the research ecosystem?”

Well, we did that. You can find the [uploaded gapminder data files on Zenodo](https://doi.org/10.5281/zenodo.14768556) and you can explore the modified lessons here:

* [Shell Novice (NIH-GREI fork)](https://nih-grei.github.io/shell-novice/)  
* [Python Gapminder (NIH-GREI fork)](https://nih-grei.github.io/python-novice-gapminder/)

## Teaching Moments and Real-World Applications

We tested these materials in April 2025 with a 1-day in-person Carpentries workshop at Georgia Tech. The feedback we received validated what we hoped: participants appreciated learning about generalist repositories, not as abstract infrastructure, but as practical tools embedded in their everyday workflows.

This integration gave us a way to:

* Talk about PIDs (Persistent Identifiers) as something learners could use immediately, not just see in metadata.  
* Introduce the idea of publishing data alongside code as part of a reproducible pipeline.  
* And reinforce open science values of transparency, reuse, and collaboration as core competencies.

## Community Reflections

As part of this project, we also launched a mini-series of polls in The Carpentries community. These quick prompts asked questions like:

“Do you know what a generalist repository is (without Googling it)?”

“Do you ever access your data programmatically from a repository?”

“Should we integrate repository tools into more Carpentries lessons?”

The results revealed both curiosity and enthusiasm. Many learners were new to generalist repositories, but overwhelmingly said they’d like to see more of this content included. The feedback reinforced that this isn’t a niche concern. It’s a shared interest.

## Looking Ahead: Toward Reusability by Design

Our work with GREI has made one thing clear: teaching people *how* to work with data also means helping them *think* about where their data lives, how it's accessed, and how it can be reused by others. As we look to the future, we hope to build on this pilot by supporting lesson Maintainers, community contributors, and Instructors who want to bring repository-aware thinking into their teaching.

If you're interested in exploring these materials or adapting them for your own lessons, we’d love to hear from you. You can read our [original blog post](https://carpentries.org/blog/2024/12/carpentries-and-grei-collaboration/), check out the modified lessons, or explore the [GREI initiative](https://datascience.nih.gov/data-ecosystem/generalist-repository-ecosystem-initiative) in more depth.