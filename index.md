---
layout: home
title: Home
---

<div id="intro-wrapper" class="l-text">
	<div id="intro-title-wrapper">
		<div id="intro-image-wrapper">
			<img id="intro-image" src="/images/portrait.png"></div>
		<div id="intro-title-text-wrapper">
			<h1 id="intro-title">Hi, I'm Pratham Mehta</h1>
			<div id="intro-subtitle">I'm a student at Georgia Tech</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<div id="everything-else" class="l-middle">
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a>
	</div>
	<div>
		I am an undergraduate student at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/gt-logo.png"> Georgia Tech, pursuing my bachelor's degree in computer science with a focus on <b><span class="cv-vis">human-computer interaction</span></b> and <b><span class="cv-ai">artifical intelligence</span></b>. I am  advised by <a href="http://www.cc.gatech.edu/~dchau/">Polo Chau</a> and my research focusses on developing augmented reality tools to facilitate better surgical planning and training for cardiovascular surgeons. 
	</div>
	<div style="height: 1rem"></div>
	<div>
		I have learnt full-stack technologies, backend tools, cloud computing services, and software development principles through my previous internships at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/tesla.png"> Tesla and <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/NCR.png"> NCR Corporation.
	</div>
</div>

<hr class="l-middle home-hr">

<h2 class="feature-title">Featured <a href="/cv/#publications">Research Publications</a></h2>

<p class="feature-text">
	Latest research for fans of human-computer interaction, data visualization, and machine learning.
</p>

<div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div>

<br>

[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[alex]: http://va.gatech.edu/endert/ "Alex Endert"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[nstrf]: https://www.nasa.gov/strg/nstrf "NASA Space Technology Research Fellowship"