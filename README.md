## The Carpentries website

This is the repo for [The Carpentries website](https://carpentries.org).  The site is built using [The Carpentries Hugo theme](https://github.com/carpentries/carpentries-hugo-theme).  

To build this site locally, follow the instructions in the theme's repo.

Run `make serve` in your project's folder to serve the site locally.

## Organizing content 

On 18 November 2024, this site was released using Hugo as the static site generator.  This README section will be updated as we add in more information about how to use the new infrastructure.

### Blog posts

Blog posts go in the `content/posts/YYYY/MM` folder.  Images for the blog posts go in the corresponding `static/blog/YYYY/MM` folder. Note YYYY is the four digit year and MM is the two digit month.  

The blog post date should be set in the file's front matter. Be sure the date and the file location match up.  

**Blog post tags:** Whenever possible, make sure the tags are from our [list of existing tags](https://carpentries.org/blog/posts-by-tags/).

