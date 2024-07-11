---
layout: page
authors: ["Karen Word", "Kelly Barnes"]
teaser: "Carpentries Core Team gets a start on alt text updates for Carpentries lessons"
title: "Core Team 'Acc-athon' to Add Alt Text Across Carpentries Curricula"
date: 2021-04-22
time: "09:00:00"
tags: ["Accessibility", "Lessons"]
---

At the end of March, the Core Team had an "Acc-athon", or accessibility hackathon, led by Erin Becker, where we worked together to add and improve alt text across
Carpentries curricula.

## What is alt text?

Alternative text or alt text is an HTML element that describes the appearance and function of an image on a page. Alt text serves several functions. It appears
in place of an image if the image is broken. It enhances the discoverability of content, because search engines can index alt text. But, perhaps most crucially,
alt text makes web content more accessible. If someone uses a screen reader, when the screen reader gets to an image, it will dictate the alt text in place
instead.  

While alt text is vital for accessibility when communicating with images, it is often overlooked. Many people do not realize it exists and most of us do not know
how to write alt text well. Images often omit alt text and, when they do include it, it is often not descriptive enough to be useful. It is common for alt text
to include only the name of the image file.   

## Why is good alt text important?

Including descriptive alt text alongside images makes content more accessible to people who:
* are blind or visually impaired,
* have sensory processing disorders,
* have slow internet connections, and
* everyone when images are broken or missing!  

Prioritising descriptive alt text that adequately conveys the meaning of an image is an important way to make web content more inclusive. Inclusivity is a [core
value of The Carpentries](https://carpentries.org/values/), so we believe that ensuring all images in our lessons have descriptive alt text creates a more welcoming space for everyone and allows
more people to learn from our lessons.

## How can we write good alt text?

The guidelines the Core Team followed during our "Acc-athon" included several basic "Dos" and "do nots" to follow. These included:

### Do

- Be descriptive
- Keep it short (100-125 characters is optimal)
- If image includes text, do include it in alt text

### Do not

- Include "image of" or "picture of" - but describing the type of image can be helpful (e.g. headshot, illustration, screenshot).
- Use images as text
- Repeat the caption
- Describe purely decorative images - but do enter something to mark the absent image

## Examples

![fluffy orange cat sleeping in a box](https://upload.wikimedia.org/wikipedia/commons/thumb/3/36/Cat_liquid.jpg/1600px-Cat_liquid.jpg)

Before commencing our work, we practiced together on a few photos (e.g. cats in boxes) and discussed the pros and cons of our various strategies.
Limiting the word count was especially challenging, as was deciding on the most important features of the image. Do you describe the color of the
cat or what it is doing in the box? How do you convey the way the fur looks like a liquid filling the box? Is it important that the cat is asleep?
Context matters! So, we were ready to get down to business with the contextualized images in our curricula.

## Acc-athon process

François created a spreadsheet with links to all of the images in Carpentries curricula that currently lacked alt text. We engaged in a 3 step process:
- One person drafts alt-text and adds it to the spreadsheet
- Another person is recruited to discuss and approve. We used Zoom breakout rooms to talk with each other as we finished drafting our text.
- Once many alt text additions had been approved in the spreadsheet, we began adding them as pull requests to the curricula on GitHub. (This was mostly done
in a second session.)

## How did we do?

In total, we submitted captions to 83 images over the course of our two acc-athon sessions. To date, 80 of these submissions have been reviewed and merged,
thanks to the prompt attention of the volunteer Maintainers of these lessons! At the beginning of our efforts, 53% of the images in Carpentries lessons
considered "stable" (as opposed to Alpha, Beta, etc.) lacked acceptable alt text, or a total of 323 images. We did not get them all, but by the end we were
down to 40%, or 239 that need work.

## How can you help?

We still have many images to work on, with help needed in English and in Spanish! Adding alt text is a quick way to make a big difference, and is an **ideal contribution for Instructor checkout!**
Not feeling qualified? Rest assured: we were totally unqualified as well. Improving on alt text submitted by Core-Team members is *also* a great way to
contribute. But keep in mind that *any* new submission is going to be better than nothing.
[Remaining images are detailed in this spreadsheet](https://docs.google.com/spreadsheets/d/11s7rzIMSlhAkNl8BKeWffnHirP7N2_E4SXFRPrArUqY/edit?usp=sharing).
When you start work on a pull request, please write "yes" in the column labeled "Claimed?" for the images you plan
to address in your PR. When your PR is submitted, please add a link to your PR in each of the rows to which it applies in the column labeled "PR link."

### Technical Guidance

Carpentries lesson pages are mostly formatted in Markdown, but occasionally you may come across some sections in HTML.

#### Markdown

Format:
```![Alt text here](image link here)```
Example:
```![Diagram illustrating use of select function to select two columns of a data frame](../fig/13-dplyr-fig1.png)```

#### HTML

Format:
```<img src="image link here" width="do not change this number" alt="Alt text here">```
Example:
```<img src="../fig/logging-onto-cloud_1.png" width="500" alt="Screenshot of AWS EC2 dashboard showing location of launch instance button.">```
