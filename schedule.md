---
layout: page
title: Schedule
description: The weekly event schedule.
---

# Weekly Schedule

The lectures begin the week starting 15th January 2024 (Week 1). 

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
