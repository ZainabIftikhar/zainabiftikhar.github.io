---
layout: page
title: Blog
permalink: blog/
---

# Blog

<p>Fun things I develop and share with the internet.</p>

<div class="posts">
  {% for post in site.categories.blog limit:5 %}
  <article class="post">
    <h2>
      <a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>

    <time datetime="{{ post.date | date: "%B %-d, %Y" }}" class="post-date">{{ post.date | date: "%B %-d, %Y" }}</time>

    {{ post.excerpt }}
  </article>
  {% endfor %}
</div>

<hr/>