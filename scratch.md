---
title: Scratch
layout: page
---

<div class="content">

    {% for post in site.scratch %}
    <div class="post-list">
        <h2 class="post-title">
      <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
    </h2>
        {% if post.description %}
        <p>{{ post.description }}</p>
        {% endif %}

        {% if post.date %}
        <div class="post-date">
            <time>{{ post.date | date_to_string }}</time>
        </div>
        {% endif %}
    </div>

    {% endfor %}

</div>
