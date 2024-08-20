---
layout: page
title: About
description: About the course
nav_order: 2
---

# About
{:.no_toc}

<!---
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## About
-->

AI Citizenship for Clinicians is an open source medical AI curriculum developed by practicing clinicians and artificial intelligence researchers. Our primary intended audience is medical practicioners (medical students, residents, attendings), whom we hope to empower to be informed users of clinical AI systems so that they may maximize the benefits and minimize the harms associated with this increasingly ubiquitous technology.

## Course Staff
### Course Directors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign contributors = site.staffers | where: 'role', 'Contributor' %}
{% assign num_contributors = contributors | size %}
{% if num_contributors != 0 %}

### Contributors

{% for staffer in contributors %}
{{ staffer }}
{% endfor %}
{% endif %}
