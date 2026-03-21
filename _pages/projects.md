---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% for proj in site.data.projects %}

{% if proj.role != "Researcher" %}

## {% if proj.acronym %}{{ proj.acronym }}: {% endif %}{{ proj.title }}
**Role:** {{ proj.role }}<br>
{{ proj.date_start }} -- {% if proj.date_end %}{{ proj.date_end }}{% else %}Present{% endif %}<br>
{%- if proj.description -%}
  {{ proj.description }}<br>
{%- endif -%}
{%- if proj.partners -%}**Partners:** {% for partner in proj.partners %}{{ partner.name }}{% if forloop.last == false %}, {% endif %}{% endfor %}<br>{%- endif -%}
{%- if proj.reference -%}**Reference:** {{ proj.reference }}<br>{%- endif -%}
{%- if proj.website -%}**Website:** <a href="{{proj.website}}">{{ proj.website }}</a>{%- endif -%}

{% endif %}
{% endfor %}

## Participation in other Research Projects

{% for proj in site.data.projects %}

{% if proj.role == "Researcher" %}

{% if proj.acronym %}{% assign proj_title = proj.acronym | append: ": " | append: proj.title %}{% else %}{ assign proj_title = proj.title %}{% endif %}

- {% if proj.website %}<a href="{{proj.website}}">{{ proj_title }}</a>{% else %}{{ proj_title }}{% endif %}
 {% if proj.reference %}({{ proj.reference }}){% endif %}{% if proj.date_end %}. {{ proj.date_start }}--{{ proj.date_end }}{% else %}. {{ proj.date_start }}--Present{% endif %}


{% endif %}
{% endfor %}
