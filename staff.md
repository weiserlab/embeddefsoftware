---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Course Staff

The course is coordinated and taught by the instructor Prof. Ambuj Varshney. The support staff helps with the troubleshooting of IoT devices and with the course logistics.

## Instructor

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}

{% assign support_staff = site.staffers | where: 'role', 'Support Staff' %}
{% assign num_support_staff = support_staff | size %}
{% if num_support_staff != 0 %}

## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}


## Support Staff

{% for staffer in support_staff %}
{{ staffer }}
{% endfor %}
{% endif %}