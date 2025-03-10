---
layout: page
authors: ["Toby Hodges"]
teaser: "Summarising the recommendations of the Lesson Setup Instructions Task Force"
title: "Updating our Lesson Setup Instructions"
Date: 2025-03-12
time: "09:00:00"
tags: ["Curriculum", "Python", "R", "Shell"]
---

The Lesson Setup Instructions Task Force was [established in August 2024 to review existing setup instructions](https://github.com/carpentries/task-forces/blob/main/2024/lesson-setup/lesson-setup-instructions.md) for Data Carpentry, Library Carpentry, and Software Carpentry lessons and decide where and how these instructions should be updated. Members of the task force considered a wide range of options for installing Bash, Git, Python, and R, and engaged in many constructive discussions. The task was challenging, and the “best” option was often difficult to identify.

**Task force members:** Toby Hodges (Chair), Rob Davey, Matt Fisher, Nathaniel Porter, Jennifer Stubbs, Adam Taranto

[The full text of the task force’s recommendations](https://github.com/carpentries/task-forces/blob/main/2024/lesson-setup/lsitf-recommendations.md) can be found in the `carpentries/task-forces` repository on GitHub. Here we provide a summary, highlighting the changes that we expect to impact Instructors the most.

1. [Add instructions to use WSL 2 for lessons taught in the Shell](#1-add-instructions-to-use-wsl-2-for-lessons-taught-in-the-shell)
2. [Continue using RStudio for now, but monitor the development of Positron](#2-continue-using-rstudio-for-now-but-monitor-the-development-of-positron)
3. [Update Python instructions to use miniforge](#3-update-python-instructions-to-use-miniforge)
4. [Add instructions to install VS Codium/VS Code for Python lessons](#4-add-instructions-to-install-vs-codiumvs-code-for-python-lessons)
5. [Teach the fundamentals of environment management in novice Python lessons](#5-teach-the-fundamentals-of-environment-management-in-novice-python-lessons)


## 1. Add instructions to use WSL 2 for lessons taught in the Shell

**Current state:** Instructions direct participants working on Windows to install [Git for Windows](https://gitforwindows.org/) (which provides the Git Bash terminal).

**After updates:** Instructions will recommend that participants working on Windows use [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/about), or install Git for Windows if they cannot access WSL 2.

**Expected impact on Instructors:** Learners’ paths may vary between Windows systems using WSL 2 and Git Bash. Learners with WSL 2 can access the manpages of commands (unavailable in Git Bash).

Git for Windows, which emulates a Linux environment on Windows systems, has served Instructors and learners well in Carpentries workshops for many years. However, Windows Subsystem Linux (WSL 2), released in 2020, provides a more complete Linux environment for Windows users. The task force felt that WSL 2 would give learners several advantages during and after the workshop, including a separate filesystem linked with access to the Windows environment and more complete options for installing additional software into their environment later.

Nevertheless, the task force determined that it was not yet right to drop support for Git for Windows altogether. We can expect some learners to join workshops with older Windows systems that cannot support WSL 2 or with systems managed by their employer on which WSL2 is not permitted. To account for this, WSL 2 will be presented as the preferred installation option on Windows systems and Git for Windows as the “fallback option” where WSL 2 is unavailable.


## 2. Continue using RStudio for now, but monitor the development of Positron

**Current state:** R lesson setup instructions recommend that learners install R Studio.

**After updates:** No change.

**Expected impact on Instructors:** No change.

Instructors have been successfully teaching lessons using R with R Studio for many years. Posit, the developers of R Studio, announced a new integrated development environment (IDE), [Positron](https://positron.posit.co/), in 2024. Although it is currently under early, rapid development and not yet ready for adoption at Carpentries workshops, the task force anticipates that Positron will replace R Studio as the IDE of choice for R users over the next few years. 

**The task force recommends that R Studio continues to be used for lessons teaching with R**. When a first stable release of Positron is made, and thereafter as needed, the Curriculum Team will revisit this and consider recommending Positron as an IDE for R and Python lessons (related to recommendation 4, below).


## 3. Update Python instructions to use miniforge

**Current state:** For most Python lessons, learners are directed to install [Anaconda](https://www.anaconda.com/download).

**After updates:** Instructions will direct learners to install [miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#miniforge), and create an environment containing the libraries required for core lessons aimed at novices.

**Expected impact on Instructors:** Learners may need additional support setting up and activating the environment for use in the workshop. Further discussion of environments may be required during workshops (see recommendation 5).

The task force considered a wide range of options for installing Python for lessons, from the currently used option, Anaconda, through a “vanilla” installation from python.org with an environment managed with pip to JupyterLab Desktop.

No strong “favourite” emerged among the various options considered by the task force. However, the choice to continue using Anaconda was discounted due to concerns that learners could inadvertently breach its terms of service by installing packages from the default channel when they continue to use Python after a workshop. Task force members also reported a loss of trust in Anaconda, Inc., following the sudden change of the ToS, enforcement actions, and associated communications last year.

It was difficult to choose between several options, but ultimately, **the task force recommends miniforge for use in Python lessons**. The distribution is set up to use conda-forge by default, eliminating concerns about learners contravening Anaconda’s terms of service after a workshop, and teaching learners the basics of how to use conda for environment management (see recommendation 5) will help learners from a wide range of disciplines continue to use their setup from a workshop long after the event has finished.

“Vanilla” Python and pip scored similarly highly to miniforge in the task force’s assessment, but ultimately, the group chose a conda-based solution due to the relative ease of its adoption: since Python lessons currently use Anaconda, several lessons already use conda for additional setup steps.

The use of a mini forge should not force Instructors to change the way that they teach Python in workshops. For example, Instructors who prefer to teach with Jupyter Notebooks can continue to do so. However, as discussed in Recommendation 4, instructions will be added for learners to set up an IDE before joining Python lessons.

The shift away from Anaconda has additional implications beyond the need to update installation instructions. Recommendation 5 describes how this change will impact the content of Python lessons for novices.


## 4. Add instructions to install VS Codium/VS Code for Python lessons

**Current state:** Python installation instructions assume that workshops will be taught with Jupyter Notebooks, and no instructions are provided for installing an IDE for Python lessons.

**After updates:** Guidance for setting up Jupyter Notebooks will be retained as the default, accompanied by instructions to install [VS Codium](https://vscodium.com/) and [VS Code](https://code.visualstudio.com/).

**Expected impact on Instructors:** Instructors will not be required to change the way they teach but will be more easily able to choose to ask learners to install an IDE for Python before a workshop.

As mentioned above, R lessons have been taught with RStudio for many years already, and **the task force recommends that The Carpentries Instructor community consider teaching Python with an IDE** too. Although some changes would be required across the lessons, the group felt that teaching Python in an IDE would reflect common modern practice, and was excited by the possibilities it opens for using the same interface to teach all lessons in a workshop (e.g. Unix shell, Python, and Git within the IDE in a Software Carpentry workshop).

Although the Curriculum Team will consider adopting Positron for this purpose at a later date (see recommendation 2), for now the task force **recommends implementing instructions to setup VS Codium for Python lessons**, accompanied by a brief explanation of the difference between the “pure open source” VS Codium and the more widely-used VS Code, with setup instructions for VS Code provided as well for those who prefer to use it. 

The task force is aware that some lessons (e.g. [Data Carpentry: Image Processing with Python](https://datacarpentry.github.io/image-processing/instructor/instructor-notes.html#working-with-jupyter-notebooks)) are designed to be taught with Jupyter, and the setup instructions for these lessons will not be changed to use an IDE. For those lessons where setup instructions are updated to include VS Codium/VS Code, members of the task force will suggest additional changes where needed to support this setup in the main lesson content.


## 5. Teach the fundamentals of environment management in novice Python lessons

**Current state:** Python lessons for novices do not discuss environments.

**After updates:** Lessons will include a minimal discussion of environments: e.g. what they are, why they are necessary, how to create one and use one, how and when to switch between them.

**Expected impact on Instructors:** Instructors will need to make time to discuss environments when teaching Python in a workshop.

The removal of Anaconda from the setup instructions for Carpentries lessons (Recommendation 3) means that the large base environment provided by that distribution will no longer be available. Instead, learners will need to create an environment and populate it with the required packages before they can follow a lesson. 

On the one hand, this presents a new challenge for Instructors: teaching novice learners the concepts and skills required to manage their Python environment (and finding room for this in an already packed workshop schedule). On the other hand, teaching learners these basics will help us ensure that we set them up to succeed in the long term after they leave a workshop. Furthermore, if we wish to move away from using Anaconda as our preferred Python distribution, there are no viable alternatives that can provide a complete base environment on learners’ local systems.

**The task force recommends that Python lessons be updated to include a minimal discussion of environments and dependencies**. If you would like to contribute to conversations about exactly what these changes should look like, please watch out for relevant messages on the `#general` channel of The Carpentries Slack or [contact the Curriculum Team](mailto:{{< param curriculum_email >}}).


## Next steps

In the coming days, task force members will open pull requests to update lesson setup instructions according to these recommendations. The Curriculum Team will invite feedback and facilitate discussion, particularly within the Instructor community, about how these changes may impact the teaching of workshops. Watch the `#general` and `#instructors` channels on Slack and the `discuss` mailing list for further details.


## Acknowledgements and an apology

Task force chair and Director of Curriculum Toby Hodges, writes: *I am hugely grateful to the other members of this task force for the collaborative and constructive spirit with which they engaged in this process. Most of these decisions were difficult to make, with few obviously correct choices presenting themselves, and the process was slower than I originally hoped. While the setup instructions will need to be revisited again, I am relieved that we have arrived at a set of recommendations that will allow the community to proceed with confidence.*

*Finally, a note to say sorry to Mpilo Khumalo, who agreed to join the task force but became isolated from most of its discussions due to my inconsiderate reliance on Slack for communication and coordination. Unfortunately, I realised my mistake too late and it was difficult for Mpilo to catch back up with the process up to that point. After discussion, we agreed that the best way to progress towards publishing the recommendations would be to remove Mpilo’s name from the list of authors.*

*I am grateful for the contributions that Mpilo was able to make and resolved to be more intentional and inclusive with the channels I use for communication among community members in future.*
