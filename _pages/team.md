---
title: "Enliten Lab - Team"
layout: gridlay
excerpt: "Enliten Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We have open positions for new PhD students, Postdocs, and Master students!** [(see openings)](https://enliten.utk.edu/openings/)

Navigate to [Faculty](#faculty), [Staff](#staff), [Graduate Students](#graduate-students), [Bachelor Students](#bachelor-students), [Alumni](#alumni), and [Visitors](#visitors). Navigate to [Group Manual](https://enliten.utk.edu/guide/).

---
## Faculty
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% if member.member_type == 'faculty' %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

---
## Staff 
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% if member.member_type == 'staff' %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

---
## Graduate Students
### 10 PhD students, 5 MS students

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% if member.member_type == 'phd_stu' or member.member_type == 'ms_stu' %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


---
## Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% if member.member_type == 'undergrad_stu' %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


---
## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  {% if member.photo %}
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  {% endif %}
  <h4>{{ member.name }}</h4>
  <i>  {{member.employment }} <br>  {{ member.alumni_role }} Alum<br> {{ member.duration }}
  {% if member.email %} <br>email: <{{ member.email }}> {% endif %} </i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

---

## Visitors

<table align="center" style="width:100%">
<col width="100%">
  <tr>
    <td>Ms. Yichao Zhang (June 2023 - August 2023), Visiting Ph.D. Student from Aalborg University, Denmark</td>
  </tr>
  <tr>
    <td>Dr. Arif Karakas (February 2008 - January 2009), Visiting Scholar from Yildiz Technical University, Turkey</td>
  </tr>
  <tr>
    <td>Dr. Yateendra Mishra (August 2008 - January 2009) Visitng Scholar from Univesity of Queensland, Australia; employer after visiting: Midwest ISO, Indianapolis, IN; currently with Queensland</td>
  </tr>
  <tr>
    <td>Dr. Yurong Wang (Sept. 2009 - August 2010), Visiting Ph.D. Student from Southeast University, China</td>
  </tr>
  <tr>
    <td>Mr. Yan Yang (Sept. 2009 - August 2010), Visiting Ph.D. Student from South China University of Technology, China</td>
  </tr>
  <tr>
    <td>Dr. Jun Xiao (Jan. 2010 - July 2010), Visiting Scholar from Tianjin University, China</td>
  </tr>
  <tr>
    <td>Dr. Xiaobo Dou (Sept. 2010 - Sept. 2011), Visiting Scholar from Southeast University, China</td>
  </tr>
  <tr>
    <td>Dr. Weibing Wang (Feb. - May 2012), Visiting Scholar from Nanjing Inst. of Technology, China</td>
  </tr>
  <tr>
    <td>Dr. Haitao Liu (Feb. - May 2012), Visiting Scholar from Nanjing Inst. of Technology, China</td>
  </tr>
  <tr>
    <td>Dr. Xianyun Li (Feb. - Aug. 2012), Visiting Scholar from Nanjing Inst. of Technology, China</td>
  </tr>
  <tr>
    <td>Ms. Fan Chen (Sept. 2013 - March 2014), Visiting Scholar from Hohai University/Nanjing Inst. of Technology, China</td>
  </tr>
  <tr>
    <td>Dr. Kai Nie (August 2013 - August 2014), Visiting Scholar from Hunan University, China</td>
  </tr>
  <tr>
    <td>Dr. Jun Li (August 2013 - August 2014), Visiting Scholar from Nanjing Inst. of Technology, China</td>
  </tr>
  <tr>
    <td>Dr. Tao Ding (December 2013 - December 2014), Visting Ph.D. student from Tsinghua University</td>
  </tr>
  <tr>
    <td>Dr. Houhe Chen (March 2014 - April 2015), Visiting Scholar from Northeast Electric Power University, China</td>
  </tr>
  <tr>
    <td>Dr. Li Guo (June 2014 - June 2015), Visiting Scholar from Tianjin University</td>
  </tr>
  <tr>
    <td>Dr. Fengzhang Luo (November 2014 - May 2015), Visiting Scholar from Tianjin University</td>
  </tr>
  <tr>
    <td>Dr. Ganyu Lv (December 2014 - December 2015), Visiting Scholar from Nanjing Inst. of Technology, China</td>
  </tr>
  <tr>
    <td>Dr. Jun Wu (January 2015 - January 2016), Visiting Scholar from Wuhan University</td>
  </tr>
  <tr>
    <td>Dr. Yonghui Sun (August 2015 - July 2016), Visiting Scholar from Hohai University</td>
  </tr>
  <tr>
    <td>Dr. Zhenkun Li (January 2016 - December 2016), Visiting Scholar from Shanghai University of Electric Power</td>
  </tr>
  <tr>
    <td>Dr. Shunfu Lin (June 2016 - June 2017), Visiting Scholar from Shanghai University of Electric Power</td>
  </tr>
  <tr>
    <td>Dr. Jun Xiao (August 2016 - August 2017), Senior Visiting Scholar from Tianjin University</td>
  </tr>
  <tr>
    <td>Mr. Haiteng Han (September 2016 - September 2017), Visiting Ph.D. Student from Southeast University</td>
  </tr>
  <tr>
    <td>Mr. Haibing Wang (August 2017 - August 2018), Visiting Ph.D. Student from Shanghai Jiaotong University</td>
  </tr>
  <tr>
    <td>Mr. Mingshen Wang (August 2017 - August 2019), Visiting Ph.D. Student from Tianjin University</td>
  </tr>
  <tr>
    <td>Mr. Jing Tu (October 2018 - October 2019), Visiting Ph.D. Student from North China Electric Power University</td>
  </tr>
  <tr>
    <td>Ms. Yunwei Shen (October 2017 - March 2019), Visiting Ph.D. Student from Southeast University</td>
  </tr>
  <tr>
    <td>Ms. Nan Zhao (October 2018 - October 2019), Visiting Ph.D. Student from Southeast University</td>
  </tr>
</table>

---
## Past Undergraduate Students
<table align="center" style="width:100%">
<col width="50%">
<col width="50%">

  <tr>
    <td>Adam Foshie: January 2016 - May 2016</td>
	<td>Kimberly Glasser: March 2016 - August 2016</td>
  </tr>
  <tr>
    <td>Chad Blaylock: March 2016 - May 2016</td>
	<td>Andrew Hnilica: Spring-Summer 2015</td>
  </tr>
  <tr>
    <td>Mwamba Bowa: Spring 2015</td>
	<td>Taylor Short: Spring 2015</td>
  </tr>
  <tr>
    <td>Stephanie Steren-Ruta: Spring 2015</td>
	<td>Drew Masters: Fall 2014 & Spring 2015</td>
  </tr>
  <tr>
    <td>Abigail Teron: Summer 2014</td>
	<td>F. Chad Harley: Fall 2013, Spring 2014 and Fall 2014</td>
  </tr>
  <tr>
    <td>Cory Raszeja: Summer 2013</td>
	<td>Cheng Zhang: Summer 2013</td>
  </tr>
  <tr>
    <td>Jason Chan: Summer 2013</td>
	<td>Daniel Cash: Spring 2013</td>
  </tr>
  <tr>
    <td>Joshua Clark: Fall 2012, Fall 2013</td>
	<td>Jacob Shelton: Summer 2012</td>
  </tr>
  <tr>
    <td>Viktor Dimitrovski: Summer 2012</td>
	<td>Shawn Cox: Summer 2012</td>
  </tr>
  <tr>
    <td>Kenson Therrien: May 2011 - May 2012</td>
	<td>David Freestate: May 2011 - January 2012</td>
  </tr>
  <tr>
    <td>Nathan Dykas: 2008-09</td>
	<td></td>
  </tr>
</table>

