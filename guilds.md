---
title: "Magtheridon EU - Guilds"
---

# Magtheridon EU - Guilds

Below is a list of some of the guilds on Magtheridon, it is not a complete list, but it could be a great place to start.

{% for guild in site.guilds %}
<article class="guild">
  <h1><a href="{{ guild.website }}">{{ guild.name }}</a></h1>
</article>
{% endfor %}
