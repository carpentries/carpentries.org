---
title: 'Home'
date: 2023-01-01T08:00:00-07:00
blocks:
- layout: select-cta
  options:
    - copy: Host a workshop
      url: /workshops/host-workshop/
    - copy: Become a member organisation
      url: /support/membership/
    - copy: Become a volunteer
      url: /community/get-involved/
    - copy: Become an Instructor
      url: /instructor-training/
- layout: hero
  title: The Carpentries teaches foundational coding and data science skills to researchers worldwide.
  image: /images/hero-background.jpg
  text_color: white
- layout: stats
  title: The Carpentries has built a community of
  stats:
    - "**{{< feed_value key=\"instructors\" feed=\"https://feeds.carpentries.org/website_stats.json\" >}}** Instructors"
    - "**{{< feed_value key=\"trainers\" feed=\"https://feeds.carpentries.org/website_stats.json\" >}}** Trainers"
    - "**{{< feed_value key=\"workshops\" feed=\"https://feeds.carpentries.org/website_stats.json\" >}}** Workshops"
    - "**{{< feed_value key=\"workshop countries\" feed=\"https://feeds.carpentries.org/website_stats.json\" >}}** Countries"
 
  cta:
    copy: Join our community
    url: '/community/'
- layout: 2-col-image-text
  image_alignment: right
  image_caption: 'Credit: Fauxels'
  image: front-page/fauxels.jpg
  title: Our volunteer-led workshops are small, hands on, and interactive.
  cta:
    copy: Find a workshop
    url: '/workshops/upcoming-workshops/'
- layout: quote-slider
  slides:
    - quote: I went from a learner to an Instructor and completely changed the trajectory of my career. It helped me find my people. ❤️
      image: testimonials/saranya_canchi_testimonial.jpg
      name: Saranya Canchi
      copy: Computational Lead, University of Michigan
    - quote: I'm pretty sure I wouldn’t be a gainfully employed climate scientist without The Carpentries. 
      image: testimonials/damien_irving_testimonial.jpg
      name: Damien Irving
      copy: Climate Data Scientist
    - quote: The Carpentries opened me up to learn things I had no idea I wanted to learn or could learn. It introduced me to a great community that made this possible.
      name: Scott Peterson
      image: testimonials/scott_peterson_testimonial.jpg
      copy: Head of the Morrison Library & Graduate Services Library, University of California, Berkeley
- layout: 2-col-image-text
  image: front-page/marcus-aurelius.jpg
  title: Subscribe to our newsletter
  subtitle: Get a roundup of events, updates, and tips every month.
  cta:
    copy: Subscribe to newsletter
    url: '/about-us/newsletter/'
- layout: logo-grid
  title: Our supporters
  copy: We are supported by our member organisations, those who sponsor workshops, as well as grants and donations from various sources.
  logos:
  - logo: sponsors/mellon.svg
    url: https://www.mellon.org/
  - logo: sponsors/moore-logo.svg
    url: https://www.moore.org/
  - logo: sponsors/alfred-sloan-logo.svg
    url: https://sloan.org/
  - logo: sponsors/chan-zuck-logo.svg
    url: https://chanzuckerberg.com/
  - logo: sponsors/posit_logo.svg
    url: https://posit.co/
  cta:
    copy: Become a sponsor
    url: 'https://carpentries.typeform.com/to/EQdv1Qx4'
---
