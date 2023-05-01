---
layout: page
title: Home
id: home
permalink: /
---

# Amateur from A to Z

<p style="padding: 3em 1em; background: #f7dfec; border-radius: 10px;">
This is the master's thesis project website of <a href="http://allegrarosenberg.com">Allegra Rosenberg</a>, completed for the Experimental Humanities program at NYU. <br> <br>This project can also be read as a long-form academic paper <a href="/essay"><b>here.</b></a></p>

<div class="intro">

  <p>What is an amateur? Today the word has a negative connotation, one of failure or shabbiness or unprofessionalism; yet it derives from the Latin meaning to love or lover—something that should be roundly positive, something to be proud of. </p>


<p>My personal interest lies in the methodology of enthusiasm: I want to look at how love and obsession allows for access to new heights and depths of knowledge. The construct of the amateur, and how it has changed throughout history, will be my lens into this phenomenon. </p>

<p>For my MA thesis, I have explored concept of the amateur by creating an Amateur Alphabet,  an A to Z compendium of moments, objects, people, and phenomena that span the history of hobbies, passion projects, and personal enthusiasm.</p>

<p>You can explore the alphabet using the interactive graph below, or by following links directly from page to page.</p>


  </div>


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
