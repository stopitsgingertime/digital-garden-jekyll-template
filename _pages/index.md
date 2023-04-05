---
layout: page
title: Home
id: home
permalink: /
---

# Amateur from A to Z 💥

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
This is the master's thesis project website of <a href="http://allegrarosenberg.com">Allegra Rosenberg</a>, completed for the Experimental Humanities program at NYU. </p>



{% include notes_graph.html %}

<hr>



<strong>Artifacts, sorted by most recent updates:</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 30 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
