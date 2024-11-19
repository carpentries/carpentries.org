---
layout: page
authors: ["Joel Nitta", "Tom Kelly", "Kozo Nishida", "Masami Yamaguchi"]
title: "First Software Carpentry Workshop in Japanese"
date: 2021-06-29
time: "00:00:00"
category: ["Community", "Internationalisation", "Curriculum", "Japan", "Online Workshops"]
---

（[このブログポストを日本語で読む](https://carpentries.org/blog/2021/06/first-japanese-r-workshop-ja/)）

We recently held the first ever [Software Carpentry (SWC)](https://software-carpentry.org/) workshop in Japanese (online). The workshop was co-hosted with [B'AI Global Forum](https://baiforum.jp/en/), a research group within the [Institute for AI and Beyond](https://beyondai.jp/?lang=en), which is a joint project between the [University of Tokyo](https://www.u-tokyo.ac.jp/en/) and [Softbank](https://www.softbank.jp/en/). The title of the workshop was ["Introduction to Data Analysis with R"](https://swcarpentry-ja.github.io/2021-04-02-todai-online-en/), with content based on the [one lesson we’ve translated so far](https://swcarpentry-ja.github.io/r-novice-gapminder/ja/), SWC "R for Reproducible Scientific Analysis"[^prev-blog]. Below, we summarize how the workshop went, using the [tried-and-true feedback format](https://datacarpentry.org/blog/2017/06/minute-cards) of "Green Sticky Notes" (things that went well) and "Red Sticky Notes" (things that didn’t go so well).

## Green sticky notes

### Close contact with co-host

Our co-host, the [B'AI Global Forum](https://baiforum.jp/en/), was instrumental in advertising the workshop and communicating with participants. This allowed us to focus on lesson content and preparation. Having a well-organized, professional co-host goes a long way towards ensuring a workshop’s success.

### Making the most of the online experience

Our workshop was held in April 2021, just about one year since Carpentries workshops started moving online because of the Covid-19 pandemic. By this time, fortunately, many Carpentries community members had posted hints and advice about how to successfully conduct workshops online[^links]. There is even [a workshop for instructors on running online workshops](https://carpentries.github.io/instructor-training-bonus-modules/01-online-workshops-module-1/index.html)! These were extremely helpful, and we highly recommend anybody else teaching an online workshop to use them. Also, most of the participants were already quite used to the online format (zoom). So we were able to have a mostly smooth online workshop, even though it was our first time.

### Practice and preparation

Although the resources mentioned above were very helpful, tips and hints alone weren’t enough to pull off a successful workshop. We had two full meetings with all members (two instructors and four helpers) and several additional practice sessions with the two instructors. Online workshops are extremely complicated and full of places where things could go wrong; these pratice sessions allowed us to spot problems that we otherwise would never have noticed. We also spent about 30 minutes after each session debriefing, which helped us correct course as the workshop progressed.

## Red sticky notes

### Some confusion about what content to teach

We had originally planned to teach SWC [R for Reproducible Scientific Analysis](http://swcarpentry.github.io/r-novice-gapminder/), since that is the only complete lesson that we've translated so far. However, the audience was mostly humanities graduate students, and we had only limited time for the workshop (5 sessions, two hours each). So we decided that the Data Carpentry (DC) [R for Social Scientists](https://datacarpentry.org/r-socialsci/) lesson would be more appropriate to learn practical skills quickly, rather than the SWC lesson, which focuses more on the fundamentals of R in detail. But since we didn't have that lesson translated yet, we ended up using our SWC translation for terminology, while teaching based on the DC R format (for example, prioritizing tidyverse over base R, etc.). It took us some time to reconfigure our teaching approach, but in the end we think this was the right choice. In the future, of course we hope to have all the other lessons translated and ready to use!

### Choosing the right amount of material to cover when teaching online

We anticipated that the online teaching format would limit the amount of material we would be able to cover, so we tried to only cover a few topics each session. However, on Day 4 we tried to teach the pipe (`%>%`), `dplyr::group_by()`, and `dplyr::summarize()`. Each of these is a significantly complicated topic that needs more time to teach to beginners, so that turned out to be a little too much. In the future we would give more time to these topics.

## Summary

Overall, we were very happy with our first workshop in Japanese. We received very positive feedback from participants about their satisfaction with the course [^survey]. There were some limitations because we only have a single lesson translated so far, but hopefully that will change soon. We are looking forward to growing the Japanese language Carpentries community, and hope you can join us!

## Find out more

Follow us on Twitter: [@swcarpentry_ja](https://twitter.com/swcarpentry_ja)

Find us on FaceBook: [carpentries.ja](https://www.facebook.com/carpentries.ja)

Find us on GitHub: [swcarpentry_ja](https://github.com/swcarpentry-ja)

Chat with the core team on the our slack channel (English or Japanese is fine). You can join from [The Carpentries in Japan slack channel](https://carpentries-jp-en.herokuapp.com/).

Anyone is welcome to contribute to translating lessons into Japanese. If you have any questions about our workflow on GitHub, please ask. We look forward to your participation!

[^prev-blog]: You can read more about [how we translated the lesson to Japanese here](https://carpentries.org/blog/2021/02/complete-R-lesson-japanese/).

[^links]: The following blog posts were very helpful: [Online Workshop Logistics and Screen Layouts](https://carpentries.org/blog/2020/06/online-workshop-logistics-and_screen-layouts/), [Recommendations for Teaching Carpentries Workshops Online](https://carpentries.org/online-workshop-recommendations/), [Mapping & Planning a Live Coding Workshop for Digital Delivery](https://carpentries.org/blog/2020/04/plan-map-live-coding-workshop/#my-personal-teaching-setup)

[^survey]: [Analysis results of the Japanese workshop survey are available here](https://github.com/swcarpentry-ja/2021-04-02-todai-assessment/blob/main/survey_report_ja.md) (Japanese only)
