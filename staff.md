---
layout: page
title: 👩‍🏫 Staff
description: A listing of all the course staff members.
nav_order: 6
---

# 👩‍🏫 Staff

## Instructor

<div class="staffer">
  <img class="staffer-image" src="/assets/staff-images/bt.jpeg" alt="Brendan Tomoschuk">

  <div>
    <h3 class="staffer-name">
      <a href="https://www.linkedin.com/in/tomoschuk/">Brendan Tomoschuk</a>
    </h3>

    <!-- Contact Information -->
    <p>
      <a href="mailto:brtomoschuk@ucsd.edu">brtomoschuk@ucsd.edu</a><br>
    </p>

    <!-- Instructor Paragraph -->
    <p>
    Brendan Tomoschuk is a senior data scientist at Cruise LLC and a lecturer in the Halıcıoğlu Data Science Institute at UC San Diego. He works on models and metrics for self-driving cars and teaches data science and statistics in his spare time. He completed his PhD at UC San Diego in Cognitive Psychology where his research focused on models and experimentation around bilingualism and second language learning.
    </p>
  </div>
</div>


## Staff

{% assign tas = site.staffers | where: 'role', 'TA' %}
{% for staffer in tas %}
{{ staffer }}
{% endfor %}

{% assign staff = site.staffers | where: 'role', 'Tutor' %}
<div class="role">
  {% for staffer in staff %}
  {{ staffer }}
  {% endfor %}
</div>
