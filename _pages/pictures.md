---
title: "Enliten Lab - Pictures"
layout: piclay
excerpt: "Enliten Lab -- Pictures"
permalink: /pictures/
---

# Pictures

![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic1.jpg){: style="width: 800px; float: center; border: 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic2.jpg){: style="width: 800px; float: center; border: 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic3.jpg){: style="width: 800px; float: center; border: 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic4.jpg){: style="width: 800px; float: center; border: 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic5.jpg){: style="width: 800px; float: center; border: 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/teampic/Group_pic6.jpg){: style="width: 800px; float: center; border: 10px"}


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
