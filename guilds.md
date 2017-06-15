---
title: "Magtheridon EU - Guilds"
---

# Magtheridon EU - Guilds

Below is a list of some of the guilds on Magtheridon, it is not a complete list, but it could be a great place to start.

<table class="table">
<thead>
  <tr>
    <th>Guild</th>
    <th>Links</th>
  </tr>
  <tr>
    <th>Raid Times</th>
    <th>Info</th>
  </tr>
</thead>
<tbody>
{% for guild in site.guilds %}
{% if guild.shortname != "lowercase-version-of-guild-name-without-spaces" %}
<tr>
  <td><a href="{{ guild.website }}" target="_blank">{{ guild.name }}</a></td>
  
  <!-- More info buttons -->
  <td></td>
</tr>
<tr>
  <td></td>
  <td><a class="btn btn-xs btn-primary pull-right" role="button" data-toggle="collapse" href="#{{ guild.shortname }}officers" aria-expanded="false" aria-controls="{{ guild.shortname }}officers">Officers</a></td>
</tr>
<tr class="collapse" id="{{ guild.shortname }}officers">
  <td colspan="2">
    <div class="well">
    Officers
    <ul>
    {% for officer in guild.officers %}
    <li>{{ officer }}</li>
    {% endfor %}
    </ul>
  </div>
  </td>
</tr>
{% endif %}
{% endfor %}
</tbody>
</table>
