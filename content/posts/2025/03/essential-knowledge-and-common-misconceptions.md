---  
layout: page  
authors: ["Toby Hodges"]  
teaser: "Summarising the discussion at February’s AI and The Carpentries community discussions."  
title: "Community Session Report: Essential Knowledge and Common Misconceptions"  
Date: 2025-03-18  
time: "09:00:00"  
tags: ["Artificial Intelligence", "Curriculum", "Workshops", "Instructors", "Community", "Community Discussions"]  
---

In February, The Carpentries hosted the second of three pairs of *AI and The Carpentries* community discussion sessions. The topic of this pair of sessions was *Essential Knowledge and Common Misconceptions*. For the Curriculum Team, the primary objective of these discussions was to identify the aspects of LLMs and their use in programming/data science that are *most important* to discuss during a Carpentries workshop. This post summarises the main points raised and the perspectives shared by community members who joined the sessions.

Are you interested in contributing to the ongoing discussion of these topics in The Carpentries community? The final pair of AI and The Carpentries sessions will take place next Tuesday, 25 March, at [12:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Carpentries+Community+Discussion&iso=20250325T1200) and [21:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Carpentries+Community+Discussion&iso=20250325T2100). [You can sign up to join these discussions on the community sessions Etherpad](https://pad.carpentries.org/community-sessions-2025). There are also active discussion threads on the \#general channel on Slack, and I encourage you to join in with either/both.

## Essential Knowledge

Despite the valid [ethical concerns raised in January’s community discussions](https://www.carpentries.org/blog/2025/02/the-ethics-of-teaching-llms-in-carpentries-workshops/), I believe that Carpentries workshops need to include some discussion of large language models (LLMs) in order to remain relevant and to prepare our learners for the current reality they will be using their new skills in. 

However, one major obstacle to this is the restricted time available: a typical Carpentries workshop lasts two days, which is already a severely limited window within which to cover all of the concepts and skills we want to teach. Considering that teaching something supplemental to the existing curriculum necessarily reduces the time available for that other content, we should be careful to make our teaching about LLMs as concise as possible: introducing learners to only the things that will be most useful for them, without straying into additional discussion at the cost of other aspects of the workshop.

Participants at the sessions considered different aspects to be most important to teach in a workshop, including:

* It is still important to understand what your code does, even (especially\!) if an LLM generated parts of it for you.  
* How LLMs work: how they are trained, what training data was used, and how a response is chosen.  
* Different ways in which generative AI tools can be used to help with coding, e.g.   
  * asking for an explanation of what some code is doing or what an error message means.  
  * translating code between languages.  
  * describing what you want to do and having the LLM generate it for you.  
* How to choose when an LLM is the appropriate tool for a given task, instead of searching the internet, for example, and why you might choose one tool over another.  
* How generative AI differs from other forms of artificial intelligence.  
* How changes to the prompt provided to an LLM can influence the output received.  
* The ethical and security implications of using LLMs.

It is not realistic to expect to teach all of these things in one of our existing Data Carpentry, Library Carpentry, or Software Carpentry workshops and still have time to cover everything else that we want to. Nevertheless, it is important that we makes space to address some aspects of this in our regular workshops. I aim to work with members of The Carpentries Incubator community to prepare additional materials that learners and Instructors could use for additional learning on these topics.

## Common Misconceptions

The second half of the community discussions focused on misconceptions that learners may have about LLMs and potential strategies that Instructors could use to identify and correct them. This will be important since misconceptions can hinder learning and must be confronted and corrected early and directly. 

When asked what misconceptions about LLMs they had encountered or had previously held themselves, participants emphasised the common misunderstanding that LLM chatbots “think” like humans do. Some participants also mentioned observing that learners often believe that previous prompts and responses do not influence the next response produced. Others mentioned the misconception that LLM chatbots are a direct and superior substitute for search engines.

The groups discussed challenges that Instructors might face when trying to diagnose and correct these misconceptions in a workshop. As discussed above, one significant challenge is the limited time available, restricting an Instructor’s ability to explore these topics in depth. If a workshop included a demonstration of an LLM in use, another challenge might be the unpredictability of responses: unlike many computing examples, an Instructor cannot rely on the same prompt producing the same output every time we use it. 

One participant highlighted that LLMs, when prompted to generate code directly, tend to work well for common and simple tasks but are more likely to include mistakes in output when prompted for more complex, real-world tasks. Given that most Carpentries workshops are aimed at novices, this raises the prospect that learners may develop unrealistic expectations during the workshop of how much they can rely on generative AI to write their code for them, discovering later that the foundational knowledge and skills we teach are still needed. As at least one participant has pointed out during these discussions, generating code with an LLM increases the importance of good debugging skills.

## Conclusion and Next Steps

Just like last time, the most immediate next step is another pair of community discussions scheduled for next week\! This time, we will learn from the experience of community members who have been teaching about and/or using LLMs in their own work. Some community members have been invited to present, but there will also be time for spontaneous contributions from participants and of course, for questions and discussion. These sessions will take place next Tuesday, 25 March, at [12:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Carpentries+Community+Discussion&iso=20250325T1200) and [21:00 UTC](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Carpentries+Community+Discussion&iso=20250325T2100) and [you can sign up to join these discussions on the community sessions Etherpad](https://pad.carpentries.org/community-sessions-2025).

As we previously discussed, the next step is to update the existing curriculum by incorporating content on LLMs and their potential applications. Based on the community discussions so far, informed by my own research and experience on the subject, I will prepare a pull request to make these changes to one of our lessons and invite feedback from community members within a defined timeframe. When those changes have been merged, I will call for help to roll out equivalent changes to the other lessons.

If you are interested in contributing to that process, please look for relevant messages on the \#general channel on Slack or contact me by direct message or [email](mailto:tobyhodges@carpentries.org).