---  
layout: page  
authors: ["Jannetta S. Steyn"]  
teaser: "Some tips on how to encourage learner completetion of Carpentries workshop surveys."  
title: "Incentivising the Completion of Workshop Surveys: Tips for Instructors"  
date: 2025-08-18  
time: "09:00:00"  
tags: ["Assessment", "Feedback", "Instructors", "Workshops"]  
---
_This blog post was first published on [Jannetta Steyn's personal blog site](https://hackmd.io/MA8b7C0KS9utV-Ca6KQsPQ?view), and  it is republished here with only slight formatting variations to ensure conformity with The Carpentries blog posts style guide._ 

---
As all Carpentries Instructors probably know, it is very hard to get people to complete workshop surveys. It was time to find a solution, but what can we do to inspire folks to complete yet another boring survey. Despite all my promises to learners that we look at and consider all the comments and feedback we get, it has been a miracle every time we get more than 50% of attendees to complete it. Giving people time, at the end of the lesson, to complete the survey helped a bit, but not much.

Fortunately, I'm a maker. Thus, when presented with a problem I immediately start thinking of something I can make to fix it. As a maker I have a 3D printer and I love printing stuff, especially stuff that are useful and not just aesthetic. So, for me, the natural thing to do is to 3D print something, at least semi-useful, that would serve as an incentive to learners to complete the survey at the end of the lesson. Key tags came to mind - those with the logo of the lesson topic we presented.

I googled 3D print designs a bit but couldn't quite find what I was looking for. Fortunately most open source software have a .svg version of their logo and the rest is relatively easy with OpenSCAD, which is my go-to design software. Now, at the end of each lesson we give folks time to complete the surveys with the promise that they can get a key ring when they are done.

In the spirit of The Carpentries, you can find the data with a graph below - created with Python. We run each lesson as a workshop. The last six workshops were concluded with the promise of a keyring if the post-workshop survey was completed before they left or a promise of being spammed if not. The mean percentage for completing workshops for the first 12 workshops were 61.769231% and 80% for the last six. I think we can safely say that bribery does work.

It might be worth to point out, to learners, that the overall statistics for workshops registered with the Carpentries are available at https://workshop-reports.carpentries.org/?aggregate-workshops. And if, as an Instructor, you wonder why you should register your workshops - keep these statistics in mind. It is used to advertise how The Carpentries contribute to research and helps strengthen our case when applying for grants and awards.

![Graph of attendance vs survey completeion rates](/blog/2025/08/completed-surveys.svg)


![3d printed keyrings made from Bash, Python Foundation, GitHub, and R logos](/blog/2025/08/icons-image.jpg)
_3d printed keyrings for the different lessons_

|Date|Pre|Post|Attended|%|
|---|---|---|---|---|
|20240130|10|7|14|50|
|20240319|10|9|12|75|
|20240423|12|10|12|83|
|20240521|7|12|17|71|
|20240625|13|12|15|80|
|20240730|8|6|14|43|
|20240924|14|6|16|38|
|20241008|12|4|16|25|
|20241022|10|10|19|53|
|20241105|21|14|21|67|
|20250121|15|8|15|53|
|20250204|16|13|20|65|
|20250218|22|22|22|100|
|20250311|18|17|22|77|
|20250325|11|10|13|77|
|20250422|15|14|19|74|
|20250506|16|14|15|93|
|20250520|12|11|14|79|

The design and print files for these keyrings are open source and can be found on one (or both) of my 3D print profile pages at:
- Makerworld: https://makerworld.com/en/@jannetta/upload
- Printables: https://www.printables.com/@tarrentaal_110298.