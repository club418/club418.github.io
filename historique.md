---
layout: default
title: Historique
permalink: /historique/
---

# 📚 Historique des événements

<ul class="agenda">
  {% assign events = site.events | sort: "date" | reverse %}
  {% for event in events %}
    {% if event.date < site.time %}
      <li>
        <strong>{{ event.date | date: "%d/%m/%Y" }}</strong>
        — <a href="{{ event.url }}">{{ event.title }}</a>
        {% if event.meetup_link %}
          • <a href="{{ event.meetup_link }}" target="_blank">Meet-up</a>
        {% endif %}
      </li>
    {% endif %}
  {% endfor %}
</ul>
