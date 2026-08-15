---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

The principal pages of this site are listed below. An
[XML sitemap](/sitemap.xml) is also available for automated indexing.

## Main pages

- [Home](/)
- [Research](/research/)
- [Publications](/publications/)
- [Talks and presentations](/talks/)
- [Teaching](/teaching/)
- [Curriculum vitae](/cv/)

## Research output

{% for post in site.publications reversed %}
- [{{ post.title }}]({{ post.url }}) — {{ post.status | default: "Publication" }}
{% endfor %}

## Talks

{% for post in site.talks reversed %}
- [{{ post.title }}]({{ post.url }}) — {{ post.venue }}
{% endfor %}

