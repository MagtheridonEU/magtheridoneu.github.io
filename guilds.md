---
title: "Magtheridon EU - Guilds"
---

# Magtheridon EU - Guilds

Below is a list of some of the guilds on Magtheridon, it is not a complete list, but it could be a great place to start.

<ul class="guilds">
{% for guild in site.guilds %}
<li class="guild">
  <a href="{{ guild.website }}" target="_blank">{{ guild.name }}</a>
  
  <a class="btn btn-xs btn-primary pull-right" role="button" data-toggle="collapse" href="#{{ guild.shortname }}officers" aria-expanded="false" aria-controls="collapseExample">Officers
  </a>

<div class="collapse" id="{{ guild.shortname }}officers">
  <div class="well">
    Officers
  </div>
</div>
  
  
</li>
{% endfor %}
</ul>
