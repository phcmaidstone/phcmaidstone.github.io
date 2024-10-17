---
permalink: /events/
layout: single
title: "Upcoming Events"
header:
  overlay_filter: "0.6"
  overlay_color: "#333"
  overlay_image: /assets/images/header-events.jpg
toc: false
---

## Upcoming Events

<ul>
  {% assign sorted_events = site.events | sort: 'date' %}
  {% for event in sorted_events %}
    {% if event.date >= site.time %}
      <li>
        <strong>{{ event.date | date: "%B %d, %Y" }}: {{ event.title }}</strong>        
        <p>{{ event.description }}</p>
      </li>
    {% endif %}
  {% endfor %}  
</ul>

## Like to host an event with us?

If you have a local event you'd like us to attend or help to faciliate, please let us know, we'd love to help.

[Get in touch](/contact/){: .btn .btn--primary}

