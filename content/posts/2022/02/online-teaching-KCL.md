---
layout: page
authors: ["Alessia Visconti", "Flavia Flaviani", "Stefania Marcotti"]
teaser: "King's College London Carpentries Instructor Team share their experience"
title: "Our tips and tricks for online workshop teaching"
date: 2022-03-01
time: "09:00:00"
tags: ["Teaching", "Carpentries Workshops"]
---

## Who we are
We are Alessia, Flavia and Stefania, part of the [King's College London Carpentries Instructor Team](https://kcl-carpentries.github.io/index.html).
We run regular Carpentries-like workshops on Unix and Git (8 so far, more to come!) and we are here to share some tips and tricks with the community!

## Background
Some background first. We teach our workshops online: we started doing so during the pandemic, but we found that the format suited our personal needs, so we are planning to keep them online for the foreseeable future. This also seems to widen accessibility for our participants, allowing extra flexibility (e.g., working from home, childcare, etc.). The Unix workshop is structured in 3 half-day sessions (3 hours each), plus an optional short exercise session (~1 hour); the Git workshop counts 2 half-day sessions plus an optional exercise session. Workshops are normally open to internal participants from King's College London and the NHS trust, however, we allow external participants in some instances (e.g., Global South collaborations).
We aim for about 15-20 participants per workshop (as we have found this to be a manageable number for online sessions), with the three of us instructing plus one or two helpers, if available. We take turns for leading the session (we all have favourite sessions/topics), but we can be flexible to cover for each other should the need arise. The instructors who are not teaching at a given time take care of breakout rooms (for individual help to participants), of questions in the chat, and of taking notes.

We use Zoom as a platform. This allows us to easily create breakout rooms (one participant + one instructor/helper when needed to solve issues), and to keep on screen the participants' list and the chat, alongside the main call window. We ask our participants to keep their cameras off to save some bandwidth, and we find the use of the Zoom reactions particularly helpful (more on this to follow!). One of the instructors not leading the session is made host of the call, so that they can manage breakout rooms; all the instructors are co-hosts in the call (helpful if one's internet connection drops).

At the beginning of the first session, after mention to the [Carpentries Code of Conduct](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html) and short introductions (e.g., name, department, ice-breaking question), we recapitulate the ways participants have to interact with us. We find this very important in the online format, to avoid talking for hours in front of an empty screen without knowing if anybody is listening on the other side!
For interacting, we use the Zoom chat (questions, problems - either to the whole group or to one of the instructors/helpers), a shared [Carpentries etherpad](https://pad.carpentries.org/) (notes, quick polls), the Zoom call itself (participants are asked to unmute themselves and ask questions if they are comfortable), and the Zoom reactions (green tick/ red cross - used for instant feedback similarly to the sticky notes for in-person sessions). In some instances, when problems arise, we might ask participants to share their screen with the whole call, especially if they incur in a problem that might be shared by others. We always make sure they are comfortable in doing so, and we offer the alternative of a breakout room with one instructor/helper in case they are not. We noticed that participants get more relaxed over subsequent sessions, just something to keep in mind!

We ask participants to have the Zoom call, the shared etherpad and the terminal open on their computer. If possible, the 2-screen setup is helpful. Some participants use 2 different devices, which has proved challenging if they have to share their screen with us but are using one device to code and another one for Zoom. Therefore, we tend to advise against this but can make do if this is the case by asking them to join the call from their second device too. This is in line with the [Carpentries recommendations for teaching workshops online](https://carpentries.org/online-workshop-recommendations/) too!

As instructors, we all use a 2-screen or 2-device setup. On top of Zoom (+ chat, + participant list to monitor reactions), the pad, and the terminal, we also have to keep open our notes (normally in markdown format, but this is personal preference) and Slack (which we use to communicate anything "behind the scenes"). To avoid mixing up, some of us keep the notes and Slack on a separate device (e.g., laptop/tablet), but this is again down to personal preferences.

We receive internal admin help for managing signup, which is performed via an internal platform (SkillsForge). We always allow for a waiting list, and we make sure to send numerous reminders before each course, as we observed this helps reducing no-shows. We ask participants to cancel their booking, should they not be willing to participate any longer, up to a week before the start of the workshop, in order to allow enough time to retrieve names from the waiting list. For late cancellation and no-shows, we have a policy for which the participant can't register for the following instance of the course.

Reminder emails before the start of the workshop also include instructions for setup (linking to the Carpentries website, such as [this page](https://swcarpentry.github.io/shell-novice/setup.html) for the Unix Shell). If we expect problems with different versions of the software (e.g., with Git), we also make sure the desired version of the software is stated (and add additional instructions on how to check for the software version).

Due to security settings and setup on university-managed machines, we sometimes incurred in problems with installations. These are dealt with in a case-by-case manner, but issues often involved lack of admin rights, double installations (the same software was installed twice with different versions), or unusual locations of the Desktop folder (e.g., on a local drive). We were recently made aware of the [Carpentries scaffolds](https://github.com/carpentries/scaffolds/blob/main/instructions/workshop-coordination.md#shell), which might also be a helpful resource in these situations.
We do not offer recording of our sessions. This choice is made in line with GDPR compliance (as participants might share their screen during the sessions) and to encourage more active engagement with the live-coding.

## Workshop structure
Each session is 3-hour long with a 10-15 minute break about half-way through. We always leave about 15 minutes at the end to allow for feedback, which we get through a "one up one down" format on the shared pad. Before the first session, instructors log into the call early, to give the opportunity to whoever had issues with software installation to get ready before we get started. At the beginning of the first session, we also run introductions, while the other two sessions start with a short recap of the previously learnt concepts/commands.

Each session is based on live-coding. The instructor leading the session shares their terminal (or other necessary windows, e.g., browser for GitHub), and participants are encouraged to code along. All the concepts/commands covered are first demonstrated with examples, and then exercises are given for participants to test their understanding. When we give solutions to exercise, we always run them step by step on our terminal, and we were given good feedback about this practice as it helps having everybody on board before moving on to the next topic. In general, we noticed exercises take much longer online than in person, so take into account you might need to allow extra time for those!

At the end of the session, we circulate the pad (where one of the instructors took notes) in pdf format with some added resources, which normally include command cheatsheets and Carpentries material, plus any useful links to solve issues that we found during the session. We prefer to avoid giving material beforehand, as we found participants often decide not to live-code along with the instructor if they already have the lesson notes. We might also add to the pad some extra exercises as "homework", but those are optional and are often exercises that we were planning to go through during the session but did not have time for.
We often received feedback regarding the need for more practical sessions after the course, so we added an optional 1-hour long session, for each workshop, in which we give participants an exercise that recapitulates many of the concepts learnt. We are available for questions throughout and before the end of the session we walk them through the solution on our terminal. We had a limited amount of participants taking advantage of this extra session, but the ones who did found it helpful to translate what they have learnt into their personal work.

## Workshop contents (Unix)
The workshop is aimed at individuals who have no experience with coding, so no pre-requisites are expected. It covers the following concepts during 3 sessions:

- how to navigate folders
- how to create and read files
- how to copy, rename, and delete files and folders
- how to use wildcards
- how to use piping and redirection
- how to build command pipelines
- how to find things
- how to use variables and loops
- how to write scripts to automate tasks.

This is equivalent to the following lessons in the [Shell Novice Carpentries material](https://swcarpentry.github.io/shell-novice/): 01 to 03 in the first session, 04 and 07 in the second, 05 and 06 in the third. You will notice a little bit of re-shuffling here, but this is just what works well for us!

## Workshop contents (Git)
The workshop is aimed at individuals who have no experience of version control but are familiar with the Unix shell (i.e., Shell Novice sessions 01 to 03). It will cover the basics of version control, how to collaborate with other people, and how to interface ourselves with GitHub. More in detail, the following concepts are covered during two sessions:

- how to set up Git on your computer
- how to create a repository
- how to track changes
- how to explore the repository history
- how to create, use, and merge branches
- how to clone a remote repository
- how to push to or pull from a remote repository
- how to collaborate to a common repository

This is equivalent to the following lessons in the [Git Novice Carpentries material](https://swcarpentry.github.io/git-novice/): 01 to 05 in the first session, 07 and 08 in the second. Moreover, some [mentions to branches](https://www.atlassian.com/git/tutorials/using-branches) are included . Similarly to Unix, you will notice a little bit of re-shuffling, but again, this is just what works well for us!

## Closing remarks
We hope that this run through our experience with teaching online Carpentries-like workshops might be helpful for other instructors! Should you have any questions for us, you can reach us at carpentries@kcl.ac.uk.
