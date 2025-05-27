---
title: Environmental Audio Documentaries
layout: page
permalink: /ead.html

---

# Environmental Audio Documentaries

text to describe

{%- assign items = site.data[site.metadata] | where_exp: 'item','item.objectid' -%}
{%- assign items-ead = items | where: 'format_original','Audio Documentary' -%}

{% for item in items-ead %}
{% include feature/audio.html objectid=item.objectid %}
{% endfor %}

