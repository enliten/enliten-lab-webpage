---
title: "Enliten Lab - Pictures"
layout: piclay
excerpt: "Enliten Lab -- Pictures"
permalink: /pictures/
---

# Pictures
- December 2023, Hooding at UTK<br>
From left: Bo, Junjie, Vince, Xiaofei, Dr. Li, Buxin, Jinning, Hang, Sufan <br>
(missing: Haoyuan, Jingzi, Mishal, and Chenchen) <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic_2023hooding.jpg){: style="width: 800px; float: center; border: 10px"}

- July 2023, General meeting at Orlando <br>
From left: Hang, Vince, Jinning, Buxin, Xin, Dr. Li, Hantao, Haoyuan, Jin, Chenchen, Yichao<br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic18.jpg){: style="width: 800px; float: center; border: 10px"}

- June 2023, in front of Min H. Kao Building<br>
Front fist row from left: Buxin, Jinning, Nicholas Parsly, Xiaofei, Dr. Li; Behind rows from left: Chenchen, Yichao, Vince, Sufan, Zack, Hang <br>
(missing: Haoyuan, Jingzi, and Mishal)
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic17.JPG){: style="width: 800px; float: center; border: 10px"}

- June 2023, Monthly group meeing<br>
From left: Hang, Nicholas Parsly, Zack, Jinning, Buxin, Vince, Sufan, Xiaofei, Chenchen, Yichao <br>
(Haoyuan is in the zoom; missing: Jingzi and Mishal) 
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic16.JPG){: style="width: 800px; float: center; border: 10px"}

- May 2022, Cookout at Tyson Park  <br>
From left: Trey Mingee, Jin, Jingzi, Jinning, Nicholas West, Vince, Qiwei, Xiaofei, Dr. Li, Hang, Buxin, Justin Martinez, Mishal's friend, Haoyuan, Mishal (missing: Nicholas Parsly) <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic14.jpg){: style="width: 800px; float: center; border: 10px"}

- April 2022, T&D meeting<br>
From left: Xiaofei, Buxin, Dr. Li, Haoyuan <br>
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic13.jpg){: style="width: 800px; float: center; border: 10px"}

- June 2021, “Beat the virus” cookout at Nicholas Ball Park <br>
From left: Ian, Mariana, Nicholas West, Haoyuan, Trey, Xiaofei, Hantao, Dr. Li, Buxin, Qiwei, Jin, Hang, Jinning, Vince (missing: Dr. Mingjian Cui and Justin Martinez)
![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic10.jpg){: style="width: 800px; float: center; border: 10px"}

- December 2020, Graduation during pandemic <br>
From left: Wei,  Dr. Li, Qingxin <br>
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
