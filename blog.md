---
title: Blogs
layout: home
permalink: /blog/
---


<div class="posts-list">
  <table class="posts-table">
    <thead>
      <td>Blog</td>
      <td>Date</td>
    </thead>
    {% for blog in site.posts %}
      <tr>
        <td>
          <a href="{{ blog.url | prepend: blog.baseurl }}">{{ blog.title }}</a>
        </td>
        <td>
          {{ blog.date | date: '%d/%m/%Y' }}
        </td>
      </tr>
    {% endfor %}
  </table>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
</div>

