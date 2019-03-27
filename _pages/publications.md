---
title: "Enliten Lab - Publications"
layout: gridlay
excerpt: "Enliten Lab -- Publications."
sitemap: false
permalink: /publications/
---


# Publications
See also the [full list](#full-list) or check out [Google Scholar](https://scholar.google.com/citations?user=Xlzr3HMAAAAJ&hl=en) and [Researchgate](https://www.researchgate.net/profile/Fangxing_Li).

## Highlights


{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p>{% for author in publi.authors %}{% if forloop.last %}& {% endif %} <em> {% assign l_name = author | split: ' ' | last %}{% assign f_name = author | split: ' ' | pop %}{{ l_name }}, {%for name in f_name%}{{name | split:'' | first}}.{% endfor%}, {% endfor %} </em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
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

<p> &nbsp; </p>


## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  {% for author in publi.authors %} {% if forloop.last %}& {% endif %} <em> {% assign l_name = author | split: ' ' | last %}{% assign f_name = author | split: ' ' | pop %}{{ l_name }}, {%for name in f_name%}{{name | split:'' | first}}.{% endfor%}, {% endfor %} </em>
  {{publi.venue}}, {{publi.year}}
  <br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
