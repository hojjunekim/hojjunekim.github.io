---
layout: about
permalink: /
title: <strong>Hojune</strong> Kim
description: Guest Student Researcher | German Aerospace Center DLR

profile:
  align: right
  image: profile.JPG
  address: #mention address

news: false
social: true
years: [2024]
---

_How can a robot effectively optimize the multi sensor data to precisely recognize the environment?_  
_How can we develop safe autonomy from perception to navigation, and control in a multi-robot system?_  

To explore these challenging questions, I am studying as an undergraduate student majoring in Aerospace Engineering at [**Seoul National University**](https://www.snu.ac.kr) advised by [Prof. Ayoung Kim](https://rpm.snu.ac.kr). Currently, I am a Guest Student Researcher at [**German Aerospace Center DLR**](https://www.dlr.de/en/rm) in Robotics and Mechatronics Institute advised by [Prof. Jinoh Lee](https://rmc.dlr.de/rm/de/staff/jinoh.lee/).

Over the span of my career, I have had the opportunity to work with some amazing robotic groups
on various robotic platforms.
I have been an exchange student at [**ETH Zürich**](https://ethz.ch/en.html),
a project intern at [Vision for Robotics Lab](https://v4rl.com). Additionally, I was a research intern in SNU [Satellite-Geophysics Lab](http://satgeo.snu.ac.kr), and organized Nationwide AI-Education Contest in [AI Tech Play](https://www.youtube.com/channel/UCfmSTxHQ6Y43XtHsQ7l_H3Q). Feel free to look for the projects I did!

I have broad research interests in Robotics, Computer Vision, and Machine Learning. In particular, my work focuses on Perception and Autonomy, with an emphasis on system design for real-world applications. If you have questions or would like to discuss ideas, don’t hesitate to reach out via [email](hojjunekim@snu.ac.kr)!
{: #publications}
<!-- <div class="post">

  {% if page.news %}
    {% include news.html %}
  {% endif %}

</div> -->
---

### __Publication__

<!-- #### __International Conference__ -->
{% for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
<div style="clear: both;"></div>
{: #projects}

---

### __Projects__


<ol class="project_list">
<li>
{% for project in site.projects %} 
<div id="{{project.key}}"  class="col three {% if project.selected %}yellow-box{% endif %}">
  <div style="clear: both;">
    <div style="">
        <img class="col bibone first"  src="{{ project.img | prepend: site.baseurl | prepend: site.url }}">
    </div>
  </div>
  <div class="col bibtwo last">
      <span class="title">{{project.title}}</span>
      <span class="affiliation">{{project.affiliation}}</span>
      <span class="position">{{project.position}}</span>
      <span class="links">
      {% if project.abstract %}
        [<a class="abstract">Abs</a>]
      {% endif %}
      {% if project.video %}
        [<a href="{{ project.video }}" target="_blank">Video</a>]
      {% endif %}
      {% if project.html %}
        [<a href="{{ project.html }}" target="_blank">Website</a>]
      {% endif %}
      {% if project.youtube %}
        [<a href="{{ project.youtube }}" target="_blank">Youtube</a>]
      {% endif %}
      {% if project.news %}
        [<a href="{{ project.news }}" target="_blank">News</a>]
      {% endif %}
      {% if project.extension %}
        [<a href="{{ project.extension }}" target="_blank">Extension</a>]
      {% endif %}
      {% if project.pdf %}
        [<a href="{{ project.pdf | prepend: '/assets/' | prepend: site.baseurl | prepend: site.url }}" target="_blank">PDF</a>]
      {% endif %}
      {% if project.supp %}
        [<a href="{{ project.supp | prepend: '/assets/documents/' | prepend: site.baseurl | prepend: site.url }}" target="_blank">Supp</a>]
      {% endif %}
      {% if project.poster %}
        [<a href="{{ project.poster | prepend: '/assets/documents/' | prepend: site.baseurl | prepend: site.url }}" target="_blank">Poster</a>]
      {% endif %}
      {% if project.slides %}
        [<a href="{{ project.slides | prepend: site.baseurl | prepend: site.url }}" target="_blank">Slides</a>]
      {% endif %}
      {% if project.code %}
        [<a href="{{ project.code }}" target="_blank">Code</a>]
      {% endif %}
      </span>
      <span class="description">{{project.description}}</span>
  </div>
  <div class="col proj_year">{{project.project_year}}</div>
</div>

{% endfor %}
</li>
</ol>

<!-- <div style="clear: both;"></div> -->
---

{: #activities}
### __Personal Activties__


<ol class="project_list">
<li>
{% for personal in site.personals %}
<div id="{{personal.key}}"  class="col three {% if personal.selected %}yellow-box{% endif %}">
  <div style="clear: both;">
    <div style="">
        <img class="col bibone first"  src="{{ personal.img | prepend: site.baseurl | prepend: site.url }}">
    </div>
  </div>
  <div class="col bibtwo last">
      <span class="title">{{personal.title}}</span>
      <span class="affiliation">{{personal.affiliation}}</span>
      <span class="position">{{personal.position}}</span>
      <span class="links">
      {% if personal.video %}
        [<a href="{{ personal.video }}" target="_blank">Video</a>]
      {% endif %}
      {% if personal.news %}
        [<a href="{{ personal.news }}" target="_blank">News</a>]
      {% endif %}
      </span>
      <span class="description">{{personal.description}}</span>
  </div>
  <div class="col proj_year">{{personal.project_year}}</div>
</div>


<!-- {% if project.redirect %}
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
{% else %} -->

<!-- <div class="project ">
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
</div> -->

{% endif %}

{% endfor %}
</li>
</ol>