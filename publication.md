---
layout: page
title: "Publications"
permalink: /publications/
---

{% assign publications_by_year = site.publications | group_by: "year" | sort: "name" | reverse %}
{% for year in publications_by_year %}
  <h2>{{ year.name }}</h2>
  {% assign sorted_pubs = year.items | sort: "title" %}
  {% for pub in sorted_pubs %}
  <p>
    <strong>{{ pub.title }}</strong><br>
    {{ pub.authors }}<br>
    {% if pub.journal %}
      <em>{{ pub.journal }}</em>{% if pub.volume %}, Vol. {{ pub.volume }}{% endif %}{% if pub.issue %}({{ pub.issue }}){% endif %}{% if pub.pages and pub.pages != "" %}, {{ pub.pages }}{% endif %}, {{ pub.year }}
      {% if pub.jurl %}
        <br><a href="{{ pub.jurl }}" target="_blank" class="btn btn-primary">Journal</a>
      {% endif %}
    {% else %}
      {{ pub.year }}
    {% endif %}
  </p>
  {% endfor %}
{% endfor %}

