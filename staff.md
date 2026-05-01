---
layout: page
title: People
description: Teams
---

# People

People behind the initiative of Critical Technical Practice

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}


{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
