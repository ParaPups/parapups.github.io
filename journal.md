---
layout: page
title: Journal
permalink: /journal/
---
<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>

	  <span>{{ post.excerpt | strip_html | truncatewords: 75 }}</span>
	  <a href="{{ post.url}}">read more</a>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
