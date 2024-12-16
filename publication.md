---
layout: page
title: "Publications"
permalink: /publications/
---

{% assign publications_by_year = site.publications | group_by: "year" | sort: "name" | reverse %}

{% for year in publications_by_year %}
   {% if year.name %}
   <h2>{{ year.name }}</h2>
   {% assign sorted_pubs = year.items | sort: "title" %}
   {% for pub in sorted_pubs %}
   <p>
   {% if pub.url %}
      <a href="{{ pub.url }}" target="_blank">{{ pub.title }}</a>
   {% else %}
      {{ pub.title }}
   {% endif %}
   <br>
   {{ pub.authors }}<br>
   {% if pub.journal %}
     <em>{{ pub.journal }}</em>
     {% if pub.volume %}, Vol. {{ pub.volume }}{% endif %}
     {% if pub.issue %}, ({{ pub.issue }}){% endif %}
     {% if pub.pages %}, pp. {{ pub.pages }}{% endif %}
     , {{ pub.year }}
   {% else %}
     {{ pub.year }}
   {% endif %}
   </p>
   {% endfor %}
{% endif %}
{% endfor %}
