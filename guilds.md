---
title: "Magtheridon EU - Guilds"
---

# Magtheridon EU - Guilds

Below is a list of some of the guilds on Magtheridon, it is not a complete list, but it could be a great place to start.

<table class="table">
<tbody>
{% for guild in site.guilds %}
<tr>

  <td><a href="{{ guild.website }}" target="_blank">{{ guild.name }}</a></td>
  
  <!-- More info buttons -->
  <td>
    <a class="btn btn-xs btn-primary pull-right" role="button" data-toggle="collapse" href="#{{ guild.shortname }}officers" aria-expanded="false" aria-controls="{{ guild.shortname }}officers">Officers</a>
  </td>
</tr>
<tr class="collapse" id="{{ guild.shortname }}officers">
  <td colspan="2">
    <div class="well">
    Officers
    {% for officer in guild.officers %}
      {{ officer }}
    {% endfor %}
  </div>
  </td>
</tr>
{% endfor %}
</tbody>
</table>
