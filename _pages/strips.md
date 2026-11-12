---
title: "Strips"
layout: collection
permalink: /strips/
collection: strips
entries_layout: grid
classes: wide
author_profile: false
---

Break Room, a comic strip by Tony Guerich and Mort.

{% assign latest = site.strips | sort: "date" | last %}
<div class="latest-strip">
  <h2>Latest: <a href="{{ latest.url | relative_url }}">{{ latest.title }}</a></h2>
  <p class="latest-strip__date">{{ latest.date | date: "%B %-d, %Y" }}</p>
  <a href="{{ latest.url | relative_url }}"><img src="{{ latest.header.teaser | relative_url }}" alt="{{ latest.excerpt | strip_html | escape }}"></a>
</div>

## All strips
