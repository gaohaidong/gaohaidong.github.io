---
layout: archive
title: "Patents"
permalink: /patents/
author_profile: true
---

## Patents

My patents and intellectual property achievements.

{% assign patents = site.patents | sort: "date" | reverse %}

{% for patent in patents %}
  <div style="margin-bottom: 25px;">
    <h3>
      <a href="{{ patent.url }}">{{ patent.title }}</a>
    </h3>

    <p>
      <strong>Inventors:</strong> {{ patent.inventors }}
      <br>
      <strong>Patent Number:</strong> {{ patent.patent_number }}
      <br>
      <strong>Status:</strong> {{ patent.status }}
      <br>
      <strong>Date:</strong> {{ patent.date | date: "%Y-%m-%d" }}
    </p>
  </div>
{% endfor %}
