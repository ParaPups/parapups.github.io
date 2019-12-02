---
layout: page
title: Journal
permalink: /journal/
---
<a href="{{ site.url }}/home">ParaPups</a> &gt;&gt; Journal

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>

	  <span>{{ post.excerpt | strip_html | truncatewords: 75 }}</span>
      <div class="read-more-wrapper">
	         <a href="{{ post.url}}">Read more &gt;&gt;&gt;</a>
      </div>
    </li>
  {% endfor %}
</ul>

<p class="rss-subscribe">Subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
