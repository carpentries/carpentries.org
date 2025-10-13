## The Carpentries website

This is the repo for [The Carpentries website](https://carpentries.org).  The site is built using [The Carpentries Hugo theme](https://github.com/carpentries/carpentries-hugo-theme).  

To build this site locally, follow the instructions in the theme's repo. Run `make serve` in your project's folder to serve the site locally.  This information is provided to give contributors the opportunity (but not the expecation) to build the site locally.  All pull requests will include a preview hosted by Netlify.

## Organizing content 

On 18 November 2024, this site was released using Hugo as the static site generator.  This README section will be updated as we add in more information about how to use the new infrastructure.

### General content

General content is in one of the folders in the `content` folder.  These folders are organized by theme.  No new files should be created in the root of the `content` folder.

### Blog posts

**File names and location**  
Blog posts go in the `content/posts/YYYY/MM` folder.  Images for the blog posts go in the corresponding `static/blog/YYYY/MM` folder. Note YYYY is the four digit year and MM is the two digit month. Be sure the file location and the blog post date as defined in the yaml metadata (see below) match up.

The file name should **not** include a date.  The file name should be entirely in lowercase and include the `.md` extension.  The file name should include alphanumeric characters and underscores only (no spaces or other punctuation or special characters).

**File metadata**

The file should begin with yaml metadata (data contained within three hyphens at the top of the file). Note that the keys are all in lowercase, and strings are represented by straight quotes (`"Name"` and not `“Name”`).  An example is below:

```
---
layout: page
authors: ["Person One", "Person Two"]
teaser: "A short line describing the post that will display on the blog list page"
title: "Blog post main title"
date: 2024-11-18
time: "09:00:00"
tags: ["Data Carpentry", "Community"]
---
```

**Blog post tags:** Please only make use of the tags from our [list of existing tags](https://docs.carpentries.org/resources/communications/select-blog-tags.html). If you feel there is a tag that fits your post, that is not in the list, please [reach out to us](mailto:community@carpentries.org).

### Formatting URLs

#### Using relative URLs

Within a website, use relative URLs, not absolute URLs.  For example:  
Use: `/community/events/`  
Not: `https://carpentries.org/community/events/`  
URLs to external websites should use the complete URL.  

#### Using site variables

For all commonly used URLs, use the [site variables as defined in this list](/blob/main/config/_default/params.yaml). Syntax: `[text goes here]({{< param link_name >}})`.  For example:  
Use: `[Instructor Training]({{< param instructor_training_curriculum >}})`    
Not: `[Instructor Training](https://carpentries.github.io/instructor-training/)`    

Open an issue if a commonly used URL is not in this list.

### Formatting buttons

Links can appear as buttons using the `{.button}` feature.  Use standard markown formatting all on one line, with the `{.button}` on a new line.  For example:
```
[Take the Survey Now](https://carpentries.typeform.com/to/123456)
{.button}
```

