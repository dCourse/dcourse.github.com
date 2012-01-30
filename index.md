---
layout: page
title: dCourse - Drupal kurzus - PTE-TTK
---
{% include JB/setup %}

# dCourse - Drupal programozó kurzus - PTE-TTK

Üdvözöllek, ez a Drupal programozó kurzus hivatalos weboldala.

Az oldalon a képzéssel kapcsolatos információkat, és később az előadások
anyagait találhatod. Kérdéseiddel bátran fordulj hozzám a
<dcourse@juhaszmarton.hu> email címen.

## Hírek

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
