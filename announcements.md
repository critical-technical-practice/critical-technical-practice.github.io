---
layout: page
title: Event Announcements
nav_exclude: true
description: A feed containing all of the event announcements.
---

# Event Announcements


{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
