---
layout: page
title: Gallery
permalink: /gallery/
---
<div id="gallery">
	{% for artpiece in site.artpieces %}
		<a href="{{ artpiece.url | prepend: site.baseurl }}">
	    	<figure class="gallery-item">
	        	<img src="{{ artpiece.img_src }}">
	        	<figcaption>
	              {{ artpiece.title }}
	        	</figcaption>
	    	</figure>
		</a>
  	{% endfor %}
</div>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
