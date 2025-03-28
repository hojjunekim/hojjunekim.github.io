---
layout: about
permalink: /
title: <strong>Hojune</strong> Kim
description: Incoming Master's Student | Stanford University

profile:
  align: right
  image: profile.JPG
  address: #mention address

news: true
social: true
years: [2024]
---

<!-- _How can a robot effectively optimize the multi sensor data to precisely recognize the environment?_  
_How can we develop safe autonomy from perception to navigation, and control in a multi-robot system?_  

To explore these challenging questions, -->
I am an incoming Master's student at <a href="https://www.stanford.edu/" target="_blank"><b>Stanford University</b></a> in Aeronautics and Astronautics. Previously, I was fortunate to work at <a href="https://www.dlr.de/en/rm" target="_blank"><b>German Aerospace Center (DLR)</b></a> under the supervision of <a href="https://rmc.dlr.de/rm/de/staff/jinoh.lee/" target="_blank">Prof. Jinoh Lee</a>. I am pursuing my B.S. degree in Aerospace Engineering at <a href="https://www.snu.ac.kr" target="_blank"><b>Seoul National University</b></a>, where I was advised by <a href="https://rpm.snu.ac.kr" target="_blank">Prof. Ayoung Kim</a> with a focus on perception.

My research centers on robot autonomy, utilizing optimization-based approaches for perception and control. I focus on trustworthy and safe-assured solutions, supported by experimental validation, and aim to expand to cooperative robots that interact with humans.

As a project intern at <a href="https://ethz.ch/en.html" target="_blank"><b>ETH Zürich</b></a>, I worked on distributed optimization for continuous-time SLAM and crowd navigation with reinforcement learning. I have also developed an autonomous car and quadcopter through student clubs. Furthermore, I co-organized a non-profit organization for AI education, <a href="https://www.youtube.com/channel/UCfmSTxHQ6Y43XtHsQ7l_H3Q" target="_blank">AI Tech Play</a>, and hosted a nationwide AI camp with an autonomous race car competition for students.

<div class="post">

  {% if page.news %}
    {% include news.html %}
  {% endif %}

</div>

---
### __Education__


<ol class="project_list">
<li style="width: 100%">
  <div class="three">
    <div class="bibtwo" style="float: left; box-sizing: border-box; width: 80%">
      <div style="font-size: 18px;"><strong>Stanford University</strong></div>
      <span><i>Incoming M.S. student in Aeronautics and Astronautics</i></span>
    </div>
    <div class="col proj_year" style="width: 20%;">Sept. 2025 - </div>
  </div>
  <div class="three">
    <div class="bibtwo" style="float: left; box-sizing: border-box; width: 80%; margin-top: 10px;">
      <div style="font-size: 18px;"><strong>Seoul National University (SNU)</strong></div>
      <span><i>B.S. in Aerospace Engineering, summa cum laude (expected)</i></span>
      <span>GPA: <b>4.00/4.00(Major)</b>, 3.91/4.00(Overall)</span>
    </div>
    <div class="col proj_year" style="width: 20%;">Mar. 2019 - Jun. 2025 (expected)</div>
  </div>
  <div class="three">
    <div class="bibtwo" style="float: left; box-sizing: border-box; width: 80%; margin-top: 10px;">
      <div style="font-size: 18px;"><strong>ETH Zürich</strong></div>
      <span><i>Visiting Student in Mechanical Engineering</i></span>
    </div>
    <div class="col proj_year" style="width: 20%;">Feb. 2024 - Aug. 2024</div>
  </div>
  <div class="three">
    <div class="bibtwo" style="float: left; box-sizing: border-box; width: 80%; margin-top: 10px;">
      <div style="font-size: 18px;"><strong>Gyeonggi Science High School for the Gifted</strong></div>
      <span>1-year early admission</span>
    </div>
    <div class="col proj_year" style="width: 20%;">Mar. 2016 - Feb. 2019</div>
  </div>
</li>
</ol>

---
{: #publications}

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

---
{: #awards_honors}

### __Awards__

<ol class="project_list">
<li>
{% for project in site.awards %} 
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

---

### __Honors__

<ol class="project_list">
<li style="width: 100%">
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="float: left; box-sizing: border-box;">
      <strong>Korea-Germany Junior Research Fellowship Support</strong>
      <span style="padding-bottom: 3px;"><i>Max Planck POSTECH/KOREA</i></span>
    </div>
    <div class="col proj_year" style="width: 45%; color: #ccc; text-align: right;">Sept. 2024</div>
  </div>
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="float: left; box-sizing: border-box;">
      <strong>Global Leadership Program Scholarship</strong>
      <span style="padding-bottom: 3px;"><i>Seoul National University</i></span>
    </div>
    <div class="col proj_year" style="width: 45%; color: #ccc; text-align: right;">Feb. 2024</div>
  </div>
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="float: left; box-sizing: border-box;">
      <strong>Certificate of Appreciation (AI Tech Play)</strong>
      <span style="padding-bottom: 3px;"><i>Deans, College of Engineering in Seoul National University</i></span>
    </div>
    <div class="col proj_year" style="width: 45%; color: #ccc; text-align: right;">Jun. 2021</div>
  </div>
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="float: left; box-sizing: border-box;">
      <strong>Kwanjeong Undergraduate Scholarship</strong>
      <span style="padding-bottom: 3px;"><i>Kwanjeong Educational Foundation</i></span>
    </div>
    <div class="col proj_year" style="width: 45%; color: #ccc; text-align: right;">Mar. 2021</div>
  </div>
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="float: left; box-sizing: border-box;">
      <strong>Undergraduate Research Internship Scholarship</strong>
      <span style="padding-bottom: 3px;"><i>Seoul National University</i></span>
    </div>
    <div class="col proj_year" style="width: 45%; color: #ccc; text-align: right;">Mar. 2021</div>
  </div>
</li>
</ol>


---

### __Patent__
<ol class="project_list">
<li style="width: 100%">
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="width: 80%; float: left; box-sizing: border-box;">
      <strong>Parking Location Tracking System</strong>
      [<a href="https://patents.google.com/patent/KR102291377B1/en" target="_blank">KR102291377B1</a>]
      <span><b><u>Hojune Kim</u></b>, Taekin Kim, Jinhwan Na, Jaeyoung Lee, Seunghwan Jeong</span>
    </div>
    <div class="col proj_year" style="width: 20%; color: #ccc; text-align: right;">2021</div>
  </div>
</li>
</ol>
{: #activities}

---

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

{% endfor %}
</li>
</ol>
