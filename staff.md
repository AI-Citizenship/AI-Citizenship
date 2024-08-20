---
layout: page
title: Staff
description: A listing of all the course staff members.
nav_order: 3
---

# Staff

Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.

## Course Directors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign contributors = site.staffers | where: 'role', 'Contributor' %}
{% assign num_contributors = contributors | size %}
{% if num_contributors != 0 %}

## Contributors

{% for staffer in contributors %}
{{ staffer }}
{% endfor %}
{% endif %}
