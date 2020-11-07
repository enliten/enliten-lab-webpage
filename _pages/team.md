---
title: "Enliten Lab - Team"
layout: gridlay
excerpt: "Enliten Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We have open positions for new PhD students, Postdocs, and Master students!** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies)

Navigate to [faculty, staff, and PhD students](#Faculty,-Staff-and-PhD-Students), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), and [past visitors](#lab-visitors).

## Faculty, Staff and PhD Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

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

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}




## Master and Bachelor Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

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

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


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
  <i>  {{member.employment }} <br>  {{ member.alumni_role }} Alumni<br> {{ member.duration }}
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


<table align="center" style="width:100%">
<col width="75%">
<col width="25%">
 <tr>
    <th>Visitors</th>
    <th>Past Undergraduate Students</th>
  </tr>
  <tr>
    <td>Dr. Arif Karakas (February 2008 - January 2009), Visiting Scholar from Yildiz Technical University, Turkey</td>
    <td>Adam Foshie: January 2016 - May 2016</td>
  </tr>
  <tr>
    <td>Dr. Yateendra Mishra (August 2008 - January 2009) Visitng Scholar from Univesity of Queensland, Australia; employer after visiting: Midwest ISO, Indianapolis, IN; currently with Queensland</td>
    <td>Kimberly Glasser: March 2016 - August 2016</td>
  </tr>
  <tr>
    <td>Dr. Yurong Wang (Sept. 2009 - August 2010), Visiting Ph.D. Student from Southeast University, China</td>
    <td>Chad Blaylock: March 2016 - May 2016</td>
  </tr>
  <tr>
    <td>Mr. Yan Yang (Sept. 2009 - August 2010), Visiting Ph.D. Student from South China University of Technology, China</td>
    <td>Andrew Hnilica: Spring-Summer 2015</td>
  </tr>
  <tr>
    <td>Dr. Jun Xiao (Jan. 2010 - July 2010), Visiting Scholar from Tianjin University, China</td>
    <td>Mwamba Bowa: Spring 2015</td>
  </tr>
  <tr>
    <td>Dr. Xiaobo Dou (Sept. 2010 - Sept. 2011), Visiting Scholar from Southeast University, China</td>
    <td>Taylor Short: Spring 2015</td>
  </tr>
  <tr>
    <td>Dr. Weibing Wang (Feb. - May 2012), Visiting Scholar from Nanjing Inst. of Technology, China</td>
    <td>Stephanie Steren-Ruta: Spring 2015</td>
  </tr>
  <tr>
    <td>Dr. Haitao Liu (Feb. - May 2012), Visiting Scholar from Nanjing Inst. of Technology, China</td>
    <td>Drew Masters: Fall 2014 & Spring 2015</td>
  </tr>
  <tr>
    <td>Dr. Xianyun Li (Feb. - Aug. 2012), Visiting Scholar from Nanjing Inst. of Technology, China</td>
    <td>Abigail Teron: Summer 2014</td>
  </tr>
  <tr>
    <td>Ms. Fan Chen (Sept. 2013 - March 2014), Visiting Scholar from Hohai University/Nanjing Inst. of Technology, China</td>
    <td>F. Chad Harley: Fall 2013, Spring 2014 and Fall 2014</td>
  </tr>
  <tr>
    <td>Dr. Kai Nie (August 2013 - August 2014), Visiting Scholar from Hunan University, China</td>
    <td>Cory Raszeja: Summer 2013</td>
  </tr>
  <tr>
    <td>Dr. Jun Li (August 2013 - August 2014), Visiting Scholar from Nanjing Inst. of Technology, China</td>
    <td>Cheng Zhang: Summer 2013</td>
  </tr>
  <tr>
    <td>Dr. Tao Ding (December 2013 - December 2014), Visting Ph.D. student from Tsinghua University</td>
    <td>Jason Chan: Summer 2013</td>
  </tr>
  <tr>
    <td>Dr. Houhe Chen (March 2014 - April 2015), Visiting Scholar from Northeast Electric Power University, China</td>
    <td>Daniel Cash: Spring 2013</td>
  </tr>
  <tr>
    <td>Dr. Li Guo (June 2014 - June 2015), Visiting Scholar from Tianjin University</td>
    <td>Joshua Clark: Fall 2012, Fall 2013</td>
  </tr>
  <tr>
    <td>Dr. Fengzhang Luo (November 2014 - May 2015), Visiting Scholar from Tianjin University</td>
    <td>Jacob Shelton: Summer 2012</td>
  </tr>
  <tr>
    <td>Dr. Ganyu Lv (December 2014 - December 2015), Visiting Scholar from Nanjing Inst. of Technology, China</td>
    <td>Viktor Dimitrovski: Summer 2012</td>
  </tr>
  <tr>
    <td>Dr. Jun Wu (January 2015 - January 2016), Visiting Scholar from Wuhan University</td>
    <td>Shawn Cox: Summer 2012</td>
  </tr>
  <tr>
    <td>Dr. Yonghui Sun (August 2015 - July 2016), Visiting Scholar from Hohai University</td>
    <td>Kenson Therrien: May 2011 - May 2012</td>
  </tr>
  <tr>
    <td>Dr. Zhenkun Li (January 2016 - December 2016), Visiting Scholar from Shanghai University of Electric Power</td>
    <td>David Freestate: May 2011 - January 2012</td>
  </tr>
  <tr>
    <td>Dr. Shunfu Lin (June 2016 - June 2017), Visiting Scholar from Shanghai University of Electric Power</td>
    <td>Nathan Dykas: 2008-09</td>
  </tr>
  <tr>
    <td>Dr. Jun Xiao (August 2016 - August 2017), Senior Visiting Scholar from Tianjin University</td>
    <td></td>
  </tr>
  <tr>
    <td>Mr. Haiteng Han (September 2016 - September 2017), Visiting Ph.D. Student from Southeast University</td>
    <td></td>
  </tr>
  <tr>
    <td>Mr. Haibing Wang (August 2017 - August 2018), Visiting Ph.D. Student from Shanghai Jiaotong University</td>
    <td></td>
  </tr>
  <tr>
    <td>Mr. Mingshen Wang (August 2017 - August 2019), Visiting Ph.D. Student from Tianjin University</td>
    <td></td>
  </tr>
  <tr>
    <td>Mr. Jing Tu (October 2018 - October 2019), Visiting Ph.D. Student from North China Electric Power University</td>
    <td></td>
  </tr>
  <tr>
    <td>Ms. Yunwei Shen (October 2017 - March 2019), Visiting Ph.D. Student from Southeast University</td>
    <td></td>
  </tr>
  <tr>
    <td>Ms. Nan Zhao (October 2018 - October 2019), Visiting Ph.D. Student from Southeast University</td>
    <td></td>
  </tr>
</table>
