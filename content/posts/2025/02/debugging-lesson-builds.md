---
layout: page
authors: ["Toby Hodges"]
teaser: "Guidance for community members working with our lesson infrastructure and GitHub Pages"
title: "Debugging Lesson Website Builds"
date: 2025-02-11
time: "09:00:00"
tags: ["Curriculum", "The Carpentries Workbench", "GitHub", "Lesson Infrastructure"]
---

[The Carpentries Workbench](https://carpentries.github.io/workbench) is a collection of tools that help community members build accessible websites from a collection of Markdown or R Markdown files.
Lesson developers and maintainers can use the Workbench to build a version of the lesson site on their own local system, and a set of [workflow descriptions](https://github.com/carpentries/actions) allows the site to be built on GitHub's cloud servers and served to the internet through [GitHub Pages](https://pages.github.com/).

![The summary view of a successful lesson build in the Actions tab of a GitHub repository](/blog/2025/02/successful-build-workflow.png)
_This is what a successful lesson build workflow looks like on GitHub. If your lesson builds do not look this, the rest of the blog post is for you!_

Although a lot of work has been done to make the Workbench easy to use, lesson developers will sometimes encounter problems with their lesson builds. This can be due to syntax errors and other issues with the content of the lesson, changes to the packages used in lessons built from R Markdown files, or problems with the infrastructure itself. 

In this post, I try to distill the experience I have gained over the last few years working with the Workbench to provide some troubleshooting strategies that community members can use when they find that their lesson will not build. The steps described here will not solve every problem you might encounter, and I still get stuck on new problems from time to time. But I believe they can be used to find the cause of most problems that lesson developers and maintainers may encounter and, if that is you, I hope that this post is helpful.

_(Note: this post is based on a response I originally shared on the `#lesson-dev` channel of The Carpentries Slack workspace. The `#lesson-dev` and `#workbench` channels are a fantastic place to lurk and ask questions if you are using the Workbench for your own projects.)_

## The Infrastructure
### Local setup
The Workbench maintenance team makes frequent updates to the infrastructure, e.g. to improve the infrastructure and fix issues that arise over time. If you are building your lesson locally, try [installing the Workbench R packages](https://carpentries.github.io/sandpaper-docs/#setup) again. If a newer version is available, it will be downloaded and installed. Try building the site again after any newer versions have been installed. If you are still encountering an error, look at the other steps below or [ask for help](#how-to-ask-for-help-with-the-workbench).

### On GitHub
The website builds on GitHub _automatically use the most recently released version of the Workbench_, but you will occasionally need to update the workflows themselves. If you are encountering errors in the build workflow on GitHub (called _01 Build and Deploy Site_), open the logs of the failed run and check in which step the error was encountered. If the error is in any of the steps other than _Setup Package Cache_ or _Deploy Site_, it is an issue with the workflows themselves. 

To solve this, run the _02 Maintain: Update Workflow Files_ workflow in the _Actions_ tab of your lesson repository to check whether the workflows need updating, and merge any pull request that is created to update your repository. Since this workflow will open a pull request on the repository if the workflows need to be updated, **it requires an access token to run**. If your lesson is in [The Carpentries Incubator](https://github.com/carpentries-incubator), [The Carpentries Lab](https://carpentries-lab.org/) or one of The Carpentries lesson programs, we will take care of this for you. Otherwise, you should [create a `SANDPAPER_WORKFLOW` token and add it to your repository](https://docs.carpentries.org/resources/curriculum/lesson-forks.html#configure-maintenance-workflows). Note that **the workflow will not fail if the token is missing**: if you are unsure whether the token is configured correctly, check the output in the _Actions_ tab.

![Output of the 02 Maintain: Update Workflow Files workflow in the Actions page of a GitHub repository when no SANDPAPER_WORKFLOW token is available on the repository. The output displays a message "Missing Token: The SANDPAPER_WORKFLOW secret is missing, invalid, or does not have the right scope (public_repo, workflow) to update the package cache. If you want to have automated pull request updates to your package cache, you will need to generate a new token." accompanied by instructions for generating and adding this token.](/blog/2025/02/missing-token-message.png)
_Seeing this output from the _02 Maintain: Update Workflow Files_ workflow? Follow the steps it describes to add the SANDPAPER_WORKFLOW token and enable automated pull requests to keep your workflows up to date._

If the _02 Maintain: Update Workflow Files_ workflow fails, or it produces no update, or the build still fails after updates have been merged, [ask for help](#how-to-ask-for-help-with-the-workbench).

## The Package Cache
Lessons with R Markdown source files are built by first executing the code chunks in those R Markdown files. This has several advantages, a big one being that you do not need to maintain output of your code examples in the lesson source: the output will be generated when the R Markdown files are run, and included in the lesson built from them. For this to work, the packages used in the code of the lesson need to be installed before it can be built. Just like the Workbench tools, the developers of these tools will frequently release newer versions of these packages, which should be kept up to date in the lesson. 

If you encounter an error in the _Setup Package Cache_ step of the site build workflow on GitHub, it is probably an issue with these R package dependencies for your lesson. Most problems at this step can be resolved by updating the versions of those packages for your project. Run the _03 Maintain: Update Package Cache_ workflow to update the package versions, and merge any pull request that has been created from it. Just like the _02 Maintain: Update Workflow Files_ workflow discussed above, **_03 Maintain: Update Package Cache_ requires the `SANDPAPER_WORKFLOW` token to open pull requests on your repository**.

If the _03 Maintain: Update Package Cache_ workflow fails, or it produces no update, or the build still fails after updates have been merged, [ask for help](#how-to-ask-for-help-with-the-workbench). Sometimes, problems with this step are the result of an issue with one of the packages used in the lesson, in which case the Curriculum Team and other members of The Carpentries community may not be able to help.

## The Lesson Build
Most of the errors described so far are related to the infrastructure, i.e. they are peripheral to the actual process of building the lesson website. But sometimes the problem is with the content we are trying to build. Syntax errors, misnamed and missing files, and mistakes in the configuration of the site and its pages, can all prevent the Workbench from building the lesson.
On GitHub, a problem with the lesson content will result in an error during the _Deploy Site_ step of the _01 Build and Deploy Site_ workflow. The Workbench provides error output, so you should read the logs of the workflow to try to figure out what is going wrong.

A great strategy in these cases is to try building the lesson locally. The GitHub Actions workflows can take a lot longer than local builds because the build process on GitHub Actions creates a new virtual machine from scratch and installs all of the required software every time before it can even start trying to build the lesson. Debugging a failing build is a lot more frustrating if you have to wait for this process to finish every time you make a change, before you can see if the error has been resolved. If you [install the Workbench tools on your local system](https://carpentries.github.io/sandpaper-docs/#setup), you can run `sandpaper::serve()` in an R session to try to build your lesson. If that fails, you can edit the files in your lesson and keep trying to build it.

If you cannot figure out what is going wrong, or you cannot get the local builds working for any other reason, [ask for help](#how-to-ask-for-help-with-the-workbench).


## How to ask for help with the Workbench
There are several different ways that you can ask for help with The Carpentries Workbench.
Possibly the best way is to post your question to the `#workbench` channel on The Carpentries Slack Workspace ([Slack invite link](https://slack-invite.carpentries.org/)). 
You can also send a message to <team@carpentries.org>, or [email me directly](mailto:tobyhodges@carpentries.org), but Slack posts are preferred because they are visible to more people who will potentially be able to help and answer questions.

To make it easier for the community to help you, please include the following information in your post:

* the error message you received
* a link to the project GitHub repository (ideally to the logs of the failing build workflow)

A link to the GitHub repository allows other community members to look at the error themselves, and clone the project to investigate the problem in more detail.

It can also help to search the message history of the `#workbench` and `#lesson-dev` Slack channels, and to look through open and closed issues on <https://github.com/carpentries/workbench> and <https://github.com/carpentries/sandpaper>, to see if anyone else has encountered the same issue before. 

Finally, you can also open an issue on your project GitHub repository, tagging me (`@tobyhodges`), and I will do my best to help you there. If you believe that you have identified the cause of the error as a problem with the Workbench tooling itself, you can open an issue at <https://github.com/carpentries/workbench> to report it.

