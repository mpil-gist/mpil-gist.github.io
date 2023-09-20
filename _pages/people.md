---
layout: page
title: People
permalink: /people/
description:
nav: true
display_categories: [Faculty, Students]
order: 1
---
<div class="people">
  <!-- Display categorized people -->
  {% for category in page.display_categories %}
    <h2 class="category">{{category}}</h2>
    {% assign categorized_people = site.people | where: "category", category %}
    {% assign sorted_people = categorized_people | sort: "sequence" %}
    <!-- Generate cards for each person -->
    <div class="grid">
      {% for people in sorted_people %}
        {% include people.html %}
      {% endfor %}
    </div>
    {% endfor %}
    <h2 class="category">Alumni</h2>
      <ul>
        <li>Hyunjin Kim (M.S., 2021-2023)</li>
        <li>Eunju Jeong (M.S., 2021-2023) → currently at Koh Young Technology</li>
      </ul>
</div>
