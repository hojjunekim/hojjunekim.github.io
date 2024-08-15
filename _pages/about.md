---
layout: about
permalink: /
title: <strong>Hojune</strong> Kim
description: Undergraduate Student | Seoul National University

profile:
  align: right
  image: profile.JPG
  address: #mention address

news: false
social: true
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018]
---

_How can robot precisely recognize the spatial information, even in multi robot system?_  
_How can we effectively collaborate the multi sensor data?_  

<!-- _How can a robot learn to use its different parts for interactions?_  
_How can we go beyond proprioception for robust mobile manipulation?_  
_What abstractions are necessary to describe multiple tasks?_  -->

To find *some* answers to the above questions, I am currently an undergraduate student at [Seoul National University](https://www.snu.ac.kr) advised by [Ayoung Kim](https://ayoungk.github.io), and a Guest Researcher at German Aerospace Center [DLR Robotics and Mechatronics](https://www.dlr.de/en/rm).

Over the span of my career, I have had the opportunity to work with some amazing robotic groups
on many different robotic platforms.
I have been a exchange student at [ETH Zürich](https://ethz.ch/en.html),
a research intern at [Vision for Robotics Lab](https://v4rl.com), and a part-time research engineer
at [J.Marple](https://jmarple.ai). Also, I did intern in SNU [Satellite-Geophysics Lab](http://satgeo.snu.ac.kr), and organized AI-Education Contest in [AI Tech Play](https://www.youtube.com/channel/UCfmSTxHQ6Y43XtHsQ7l_H3Q). During my student club activity, I participated in International Autonomous Driven Car Competition, and Autonomous Flight Drone Competition.

<!-- During my undergrad at [IIT Kanpur](http://www.iitk.ac.in/ee/), I was a visiting student at
University of Freiburg, Germany, working closely with [Abhinav Valada](http://www2.informatik.uni-freiburg.de/~valada/) and [Wolfram Burgard](http://www2.informatik.uni-freiburg.de/~burgard/).
I also founded the [AUV-IITK](https://auv-iitk.github.io/#/landing-page) team, where I worked on different
hardware and software aspects of building an autonomous underwater vehicle. -->

If you have questions or would like to discuss ideas, feel free to reach out through
[email](hojjunekim@snu.ac.kr)!

<!-- _Shameless promotion:_  
For undergrad/graduate students at [ETH Zurich](https://ethz.ch/en.html): In case you are looking for semester projects or master thesis, please check [here](https://rsl.ethz.ch/education-students.html) for available projects with me and other amazing people in our group! -->

<div class="post">

  {% if page.news %}
    {% include news.html %}
  {% endif %}

</div>

---

{: #publications}
## __Publications__

{% for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}