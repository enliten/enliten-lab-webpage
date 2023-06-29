---
title: "Enliten Lab - Pictures"
layout: piclay
excerpt: "Enliten Lab -- Pictures"
permalink: /pictures/
---

# Pictures

- June 2023, (missing: Haoyuan Sun, Jingzi Liu, and Mishal Alonize) <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic17.JPG){: style="width: 800px; float: center; border: 10px"}

- June 2023, Monthly group meeing (Haoyuan is in the zoom; missing: Jingzi Liu and Mishal Alonize) <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic16.JPG){: style="width: 800px; float: center; border: 10px"}

- May 2022, Cookout at Tyson Park (missing: Nicholas Parsly) <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic14.jpg){: style="width: 800px; float: center; border: 10px"}

- Aprl 2022, T&D meeting<br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic13.jpg){: style="width: 800px; float: center; border: 10px"}

- June 2021, “Beat the virus” cookout at Nicholas Ball Park (missing: Dr. Mingjian Cui and Justin Martinez) <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic10.jpg){: style="width: 800px; float: center; border: 10px"}

- December 2020, Graduation during pandemic <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic11.jpg){: style="width: 800px; float: center; border: 10px"}

- December 2019, Year-end and graduation party with friends and collaborators at Wasabi restaurant <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic09.jpg){: style="width: 800px; float: center; border: 10px"}

- December 2019, Year-end and graduation party with friends and collaborators at Wasabi restaurant<br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic08.jpg){: style="width: 800px; float: center; border: 10px"}

- September 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic07.jpg){: style="width: 800px; float: center; border: 10px"}

- September 2019, Monthly group meeting <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic06.jpg){: style="width: 800px; float: center; border: 10px"}

- August 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic04.jpg){: style="width: 800px; float: center; border: 10px"}

- April 2018, EECS Award Banquet (Hantao Cui and Qingxin Shi received Outstanding GRA awards and Mariana Kamel received Outstanding GTA award) <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic15.jpg){: style="width: 800px; float: center; border: 10px"}

- December 2016 - Three generations of professors: Prof. Hantao Cui (now at Oklahoma State), Prof. Li, and Prof. Robert Broadwater (Virginia Tech, Dr. Li’s former advisor), from left to right. <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic12.jpg){: style="width: 800px; float: center; border: 10px"}

- December 2015, Hooding ceremony with Drs. Qinran Hu, Xue Li, and Kumar Prabakar   <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic03.jpg){: style="width: 800px; float: center; border: 10px"}

- October 2015 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic02.jpg){: style="width: 800px; float: center; border: 10px"}

- April 2015 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic01.jpg){: style="width: 800px; float: center; border: 10px"}

{% assign number_printed = 0 %}

{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>
