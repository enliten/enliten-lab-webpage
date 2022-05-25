---
title: "Enliten Lab - Pictures"
layout: piclay
excerpt: "Enliten Lab -- Pictures"
permalink: /pictures/
---

# Pictures

- Apr. 2022 - T&D meeting<br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic13.jpg){: style="width: 800px; float: center; border: 10px"}

- Jun. 2021 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic10.jpg){: style="width: 800px; float: center; border: 10px"}

- Dec. 2020 – Graduation during pandemic <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic11.jpg){: style="width: 800px; float: center; border: 10px"}

- Dec. 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic09.jpg){: style="width: 800px; float: center; border: 10px"}

- Dec. 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic08.jpg){: style="width: 800px; float: center; border: 10px"}

- Sept. 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic07.jpg){: style="width: 800px; float: center; border: 10px"}

- Sept. 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic06.jpg){: style="width: 800px; float: center; border: 10px"}

- Aug. 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic05.jpg){: style="width: 800px; float: center; border: 10px"}

- Aug. 2019 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic04.jpg){: style="width: 800px; float: center; border: 10px"}

- Dec. 2016 - Three generations of professors: Prof. Hantao Cui (now at Oklahoma State), Prof. Li, and Prof. Robert Broadwater (Virginia Tech, Dr. Li’s former advisor), from left to right. <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic12.jpg){: style="width: 800px; float: center; border: 10px"}

- Dec. 2015 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic03.jpg){: style="width: 800px; float: center; border: 10px"}

- Oct. 2015 <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic02.jpg){: style="width: 800px; float: center; border: 10px"}

- Apr. 2015 <br>
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
