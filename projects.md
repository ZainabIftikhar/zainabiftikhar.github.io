---
layout: page
title: Projects
permalink: projects/
---

# Research Projects

<p> Things I've developed involved in a mix of stuff, including research, academic course projects, and side interests. </p>

<div class="posts">
  {% for post in site.categories.projects %}
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