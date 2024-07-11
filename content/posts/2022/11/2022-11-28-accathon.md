---
layout: page
authors: ["Brynn Elliott", "Erin Becker"]
teaser: "With support from the community, we added alt text to 55 images across our lessons."
title: "Community Helps Add Alt Texts to our Lesson Images"
date: 2022-11-23
time: "09:00:00"
tags: ["Accessibility"]
---

In early September, Brynn Elliott, Accessibility Manager for The Carpentries hosted two Themed Discussions for the community focused on improving accessibility of our lessons through improving alt text on images. The group started off with an overview of what alt text is, why it is important, and how to add it to images in our lessons.## What is alt text?
Alt text - also known as alternative text, alt tags, or alt descriptions - are a written description of the image that has several purposes. Alt text is important for accessibility, screen readers can only read text, individuals who are blind or have low vision are still able to understand the image purpose. Search engine crawlers use alt text to index data and improve search results. Images that are broken or missing can still be interpreted because text is shown in its place. Alt text may vary depending on the goal of the photo.

![Sample of how alt text is displayed for a missing image.]({{ site.urlimg }}/blog/2022/11/image2.png) <br /> *Sample of how alt text is displayed for a missing image.*

## How to write good alt text
Do:
* Be descriptive
* Be short - 125 words or less
* Include text from image
* Include type of image, headshot, illustration, graph

Don’t
* Include “image of” or “picture of”
* Use images as text
* Repeat the caption
* Describe purely decorative images - but do enter something to mark the absent image

## Alt Texts for Charts and Graphs
Charts can be complicated. It is challenging to grasp the full concept of a chart in just a few short words. Amy Cesal, co-founder of the Data Visualization Society, created a template that we have adopted for The Carpentries images: [Writing Alt Text for Data Visualization](https://medium.com/nightingale/writing-alt-text-for-data-visualization-2a218ef43f81)

Alt = chart type of type of data where reason for including the chart

Example:<br />
![Example of chart to illustrate best practices for writing chart alt text.]({{ site.urlimg }}/blog/2022/11/image3.png)

Alt= (chart type) Scatter plot of (type of data) hindfoot length versus weight with transparent dots, (reason for including the chart) showing that the lower left quadrant is densely overplotted.  

## Our process
After introducing community members to the whys and hows of creating alt text, we worked collaboratively to add alt text to images across our lessons.
- Erin Becker and Zhian Kamvar, members of The Carpentries Core Team worked together to create a spreadsheet of images from our curricula. These showed which images did and did not have alt text.
- Community members who joined the discussion drafted alt text for an image and added it to the spreadsheet.
- A second person reviewed and approved the alt text.
- The alt text was added to the lesson on GitHub through a Pull Request, which was reviewed and merged by the Lesson Maintainer.

## How did we do?
We are making steady progress towards having good alt text for all of our lesson images. Prior to [our first Acc-athon](https://carpentries.org/blog/2021/04/Acc-athon/), in early 2021, 53% of images in our official stable lessons lacked acceptable alt text, or a total of 323 images. By April 2021, this number was down to 40% (239 images). Between April 2021 and September 2022, contributions from community members further improved accessibility of our images, reducing the number needing alt text to 24% (150 images). The latest acc-athon resulted in alt text being added or improved for 55 images, leaving us with 95 images still needing alt text (or about 15%

## How can you help?
We have made even more progress, however, we still have more work to do. We need your help for images in the curriculum in both English and Spanish. Alt text is such an important addition and would be a great lesson contribution for Instructor checkout! There are several ways you can check to see if images have alt text: 1. Right click on the image, select “Inspect” or “Inspect Element” and check the code for alt text, 2. Turn on a screen-reader and select the picture and hear how it is described, 3. Turn off images for webpage, (this can be found in your browser settings) alt text will show instead of the image.  If there is no alt text, the image could appear like this:
![Sample of how broken image renders without alt text]({{ site.urlimg }}/blog/2022/11/image1.png)

## Technical Guidance
### Markdown
Format: `![Alt text here](image link here) Example: ![Diagram illustrating use of select function to select two columns of a data frame](../fig/13-dplyr-fig1.png)`

_[Update June 2023: the syntax for adding alternative text to images has changed since this blog post was published.
When the new lesson infrastructure, [The Carpentries Workbench](https://carpentries.github.io/workbench/), was introduced in May 2023, 
the syntax for describing an image in the source file of a lesson became:
`[Optional caption text for image goes here](path/to/image/file/goes/here){alt='alternative text description goes here'}`]_

### HTML
Format: `<img src="image link here" width="do not change this number" alt="Alt text here"> Example: <img src="../fig/logging-onto-cloud_1.png" width="500" alt="Screenshot of AWS EC2 dashboard showing location of launch instance button.">`

### R Markdown
```{r, fig.alt = "alt text here”}```

### Workbench
[The Carpentries Workbench - Transition Guide: From Styles to Workbench ](https://carpentries.github.io/workbench/transition-guide.html#figures)
