---
title: Test Page
---

{% for post in posts %}
<div class="md-card">
  <div class="md-card__inner md-typeset">
    <h2 class="md-card__title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="md-card__content">{{ post.summary }}</p>
    <div class="md-card__actions">
      <a href="{{ post.url }}" class="md-button">Read more</a>
    </div>
  </div>
</div>
{% endfor %}