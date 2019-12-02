---
layout: page
title: Gallery
permalink: /gallery/
---
<a href="{{ site.baseurl }}/home">ParaPups</a> &gt;&gt; Gallery

<div id="gallery">
	{% for artpiece in site.artpieces %}
    	<figure class="gallery-item">
			<a href="{{ artpiece.url | prepend: site.baseurl }}">
	        	<img src="{{ artpiece.img_src }}">
	        	<figcaption>
	              {{ artpiece.title }}
	        	</figcaption>
			</a>
    	</figure>
  	{% endfor %}
</div>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
