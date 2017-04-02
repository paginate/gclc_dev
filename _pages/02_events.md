---
layout: page
title: Events
permalink: /calendar/
type: info
calendar: true
---

<ul>
  {% for event in site.posts %}
    {% if event.categories contains 'events' %}
      <li>
        <a href="{{ event.url }}">{{ event.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

<br>

Calendar of Upcoming Events

<div class="span9">
	<iframe src="http://www.google.com/calendar/embed?showTitle=0&amp;showCalendars=0&height=600&amp;wkst=1&amp;hl=en&amp;bgcolor=%23FFFFFF&amp;src=9a1j8d5duehuk7om25p46qpqic%40group.calendar.google.com&amp;color=%23AB8B00&amp;ctz=America%2FLos_Angeles" style=" border-width:0 " width="800" height="400" frameborder="0" scrolling="no"></iframe>
</div><!--/span-->