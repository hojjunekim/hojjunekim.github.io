---
layout: classic
permalink: /
title: Hojune Kim
description: Incoming Master's Student | Stanford University
profile:
  image: profile.JPG
years: [2026, 2024]
---

<p class="pageheading"><strong>Hojune</strong> Kim</p>

<div class="toprow">
  <div class="topphoto">
    <img src="{{ '/assets/img/profile.JPG' | prepend: site.baseurl | prepend: site.url }}" alt="Hojune Kim">
    <p class="toplinks">
      | <a href="{{ '/assets/documents/CV_HJ.pdf' | prepend: site.baseurl | prepend: site.url }}" target="_blank">CV</a> |
      <a href="mailto:{{ site.email }}">Email</a> |
      <a href="https://scholar.google.com/citations?user={{ site.scholar_authorid }}" target="_blank">Google Scholar</a> |<br>
      | <a href="https://github.com/{{ site.github_username }}" target="_blank">Github</a> |
      <a href="https://www.linkedin.com/in/{{ site.linkedin_username }}" target="_blank">LinkedIn</a> |
      <a href="https://x.com/HojuneKim" target="_blank">X</a> |
    </p>
  </div>
  <div class="topbio">
    <p>I am a Master's student in Aeronautics and Astronautics at <a href="https://www.stanford.edu/" target="_blank"><b>Stanford University</b></a>, advised by <a href="https://profiles.stanford.edu/mac-schwager" target="_blank">Prof. Mac Schwager</a> in the <a href="https://msl.stanford.edu/" target="_blank">Multi-Robot Systems Lab (MSL)</a>. Previously, I was a guest researcher on the humanoid TORO team at the <a href="https://www.dlr.de/en/rm" target="_blank"><b>German Aerospace Center (DLR)</b></a> and a visiting student at <a href="https://ethz.ch/en.html" target="_blank"><b>ETH Zürich</b></a>. I received my B.S. in Aerospace Engineering from <a href="https://www.snu.ac.kr" target="_blank"><b>Seoul National University</b></a>, advised by <a href="https://rpm.snu.ac.kr" target="_blank">Prof. Ayoung Kim</a>.</p>
    <p>My research bridges model-based knowledge with data-driven learning to overcome data scarcity for robot autonomy.</p>
    <p>Email: hojune [AT] stanford.edu</p>
  </div>
</div>

---
{: #publications}

### __Publication__

<!-- #### __International Conference__ -->
{% for y in page.years %}
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
<div style="clear: both;"></div>

---
### __Education__


<ol class="project_list">
<li style="width: 100%">
  <div class="three">
    <div class="bibtwo" style="float: left; box-sizing: border-box; width: 80%">
      <div style="font-size: 18px;"><strong>Stanford University</strong></div>
      <span><i>M.S. in Aeronautics and Astronautics</i></span>
      <span>GPA: <b>4.00/4.00</b></span>
    </div>
    <div class="col proj_year" style="width: 20%;">Sept. 2025 - Present</div>
  </div>
  <div class="three">
    <div class="bibtwo" style="float: left; box-sizing: border-box; width: 80%; margin-top: 10px;">
      <div style="font-size: 18px;"><strong>Seoul National University (SNU)</strong></div>
      <span><i>B.S. in Aerospace Engineering, summa cum laude</i></span>
      <span>GPA: <b>4.00/4.00(Major)</b>, 3.91/4.00(Overall)</span>
    </div>
    <div class="col proj_year" style="width: 20%;">Mar. 2019 - Jun. 2025</div>
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

{: #projects}

---

### __Projects__


<ol class="project_list">
<li>
{% for project in site.projects %}{% unless project.category == "volunteer" %} 
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
{% endunless %}
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

### __Scholarship__

<ol class="project_list">
<li style="width: 100%">
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="float: left; box-sizing: border-box;">
      <strong>Chungsoo Overseas Scholarship</strong>
      <span style="padding-bottom: 3px;"><i>Chungsoo Scholarship Foundation</i></span>
    </div>
    <div class="col proj_year" style="width: 45%; color: #ccc; text-align: right;">2025 - 2027</div>
  </div>
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
  <div class="three {% if personal.selected %}yellow-box{% endif %}">
    <div class="bibtwo" style="width: 80%; float: left; box-sizing: border-box;">
      <strong>Document editing system supporting online document creation with search function</strong>
      [KR100143446]
      <span><b><u>Hojune Kim</u></b>, Jinsu Choi</span>
    </div>
    <div class="col proj_year" style="width: 20%; color: #ccc; text-align: right;">2022</div>
  </div>
</li>
</ol>
{: #activities}

---

### __Fun Facts__


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

---

### __Volunteer__


<ol class="project_list">
<li>
{% for project in site.projects %}{% if project.category == "volunteer" %}
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
      {% if project.video %}
        [<a href="{{ project.video }}" target="_blank">Video</a>]
      {% endif %}
      {% if project.html %}
        [<a href="{{ project.html }}" target="_blank">Website</a>]
      {% endif %}
      {% if project.youtube %}
        [<a href="{{ project.youtube }}" target="_blank">Youtube</a>]
      {% endif %}
      </span>
      <span class="description">{{project.description}}</span>
  </div>
  <div class="col proj_year">{{project.project_year}}</div>
</div>
{% endif %}{% endfor %}
</li>
</ol>
