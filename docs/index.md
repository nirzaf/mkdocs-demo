# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

---
title: Home
---

# Welcome to My Site

<!-- Other content for your homepage -->

## Recent Blog Posts

<div class="md-content">
  <div class="blog-grid">
    {% for article in collections.blog %} 
    <div class="blog-card">
      <a href="{{ article.url | url }}">
        <h2>{{ article.title }}</h2> 
        <p>{{ article.summary }}</p>
      </a>
      <p class="blog-date">{{ article.date | date(format="%B %d, %Y") }}</p>
    </div>
    {% endfor %} 
  </div>
</div>