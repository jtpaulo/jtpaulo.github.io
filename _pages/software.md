---
layout: archive
title: ""
permalink: /software/
author_profile: true
---

{% include base_path %}

# Software

{% for tool in site.data.software %}
<h3><span><a href="{{ tool.url }}">{{ tool.name }}</a>
{% if tool.url %}<a href="{{ tool.url }}"><i class="fas fa-fw fa-laptop-code zoom"></i></a>{% endif %}
{% if tool.website %}<a href="{{ tool.website }}"><i class="fas fa-fw fa-globe zoom"></i></a>{% endif %}
</span></h3>
{{ tool.description }}<br>
<hr>
{% endfor %}
