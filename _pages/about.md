---
layout: about
permalink: /
title: <strong>Hojune</strong> Kim
description: Aerospace Engineering | Seoul National University

profile:
  align: right
  image: profile.JPG
  address: #mention address

news: false
social: true
years: [2024]
---

_How can a robot precisely recognize spatial information, even in a multi-robot system?_  
_How can we effectively collaborate on multi sensor data?_  

<!-- _How can a robot learn to use its different parts for interactions?_  
_How can we go beyond proprioception for robust mobile manipulation?_  
_What abstractions are necessary to describe multiple tasks?_  -->

To explore these challenging questions, I am studying as an undergraduate student majoring in Aerospace Engineering at [Seoul National University](https://www.snu.ac.kr) advised by [Ayoung Kim](https://ayoungk.github.io). Currently, I am a Guest Researcher at German Aerospace Center [DLR Robotics and Mechatronics](https://www.dlr.de/en/rm).

Over the span of my career, I have had the opportunity to work with some amazing robotic groups
on various robotic platforms.
I have been an exchange student at [ETH Zürich](https://ethz.ch/en.html),
a research intern at [Vision for Robotics Lab](https://v4rl.com). Additionally, I was a research intern in SNU [Satellite-Geophysics Lab](http://satgeo.snu.ac.kr), and organized Nationwide AI-Education Contest in [AI Tech Play](https://www.youtube.com/channel/UCfmSTxHQ6Y43XtHsQ7l_H3Q). Feel free to look for the [projects](http://hojjunekim.github.io/#projects/) I did!

If you have questions or would like to discuss ideas, don't hesitate to reach out through
[email](hojjunekim@snu.ac.kr)!
{: #publications}

<!-- <div class="post">

  {% if page.news %}
    {% include news.html %}
  {% endif %}

</div> -->
---

## __Publication__

{% for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
<div style="clear: both;"></div>
{: #projects}

---

## __Projects__

{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %}

<div style="clear: both;"></div>