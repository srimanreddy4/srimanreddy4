---
layout: default
permalink: /blog/
title: Blog
nav: true
nav_order: 3
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 5
  sort_field: date
  sort_reverse: true
---

<div class="post">
  {% if site.blog_name or site.blog_description %}
    <div class="header-bar">
      <h1>{{ site.blog_name }}</h1>
      <h2>{{ site.blog_description }}</h2>
    </div>
  {% endif %}

  {% assign featured_posts = site.posts | where: "featured", "true" %}
  {% if featured_posts.size > 0 %}
    <div class="container featured-posts">
      <div class="row row-cols-{% if featured_posts.size <= 2 or featured_posts.size % 2 == 0 %}2{% else %}3{% endif %}">
        {% for post in featured_posts %}
          <div class="col mb-4">
            <a href="{{ post.url | relative_url }}">
              <div class="card hoverable">
                <div class="row g-0">
                  <div class="col-md-12">
                    <div class="card-body">
                      <h3 class="card-title text-lowercase">{{ post.title }}</h3>
                      <p class="card-text">{{ post.description }}</p>
                      {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
                      <p class="post-meta">{{ read_time }} min read &nbsp; &middot; &nbsp; {{ post.date | date: "%Y" }}</p>
                    </div>
                  </div>
                </div>
              </div>
            </a>
          </div>
        {% endfor %}
      </div>
    </div>
    <hr>
  {% endif %}

  <ul class="post-list">
    {% if page.pagination.enabled %}
      {% assign postlist = paginator.posts %}
    {% else %}
      {% assign postlist = site.posts %}
    {% endif %}

    {% for post in postlist %}
      {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
      {% assign year = post.date | date: "%Y" %}

      <li>
        <h3>
          {% if post.redirect == blank %}
            <a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
          {% elsif post.redirect contains '://' %}
            <a class="post-title" href="{{ post.redirect }}" target="_blank">{{ post.title }}</a>
          {% else %}
            <a class="post-title" href="{{ post.redirect | relative_url }}">{{ post.title }}</a>
          {% endif %}
        </h3>
        <p>{{ post.description }}</p>
        <p class="post-meta">{{ read_time }} min read &nbsp; &middot; &nbsp; {{ post.date | date: '%B %d, %Y' }}</p>
      </li>
    {% endfor %}
  </ul>

  {% if page.pagination.enabled %}
    {% include pagination.liquid %}
  {% endif %}
</div>