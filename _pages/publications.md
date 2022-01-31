---
layout: page  
title: publications  
index: 2  
permalink: /publications/  
sections: [Conference Papers, Journals, Workshop Papers, Theses]  
nav: true
---

You can also check my [Google Scholar](https://scholar.google.com/citations?user=bsj7GpoAAAAJ) page.

<div class="publications">

{% for y in page.sections %}
  <h2 class="section">{{y}}</h2>
  {% bibliography -f papers -q @*[section={{y}}]* %}
{% endfor %}

</div>
