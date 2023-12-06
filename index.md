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
			<div id="intro-subtitle">I'm an undergraduate student at Georgia Institute of Technology</div>
			<div id="intro-title-socials">
				{% for link in site.data.social-links %}
					{% if link.on-homepage == true %}
						{% include social-link.html link=link %}
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<!-- <hr class="l-middle home-hr"> -->
	<div id="everything-else" class="l-middle">
		<a href="{{ site.url }}/cv"><div><i class="fa fa-portrait icon icon-right-space"></i>CV</div></a>
		<a href="{{ site.url }}/projects"><div><i class="fa fa-shapes icon icon-right-space"></i>Projects</div></a>
		<!-- <a href="{{ site.url }}/everything-else"><div><i class="fa fa-list-ul icon icon-right-space"></i>Everything Else</div></a> -->
	</div>
	<!-- <div>
		I design and develop interactive interfaces to help people <b>understand machine learning models</b> and data-driven systems. Besides building tools, I also create <b>data visualizations</b> and write interactive articles to simply communicate complex ideas.
	</div>
	<div style="height: 1rem"></div> -->
	<div>
		I am an undergraduate student at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/gt-logo.png">The Georgia Institute of Technology, pursuing my bachelor's degree in computer science with a focus on <b><span class="cv-vis">human-computer interaction</span></b> and <b><span class="cv-ai">artifical intelligence</span></b>. I am  advised by <a href="http://www.cc.gatech.edu/~dchau/">Polo Chau</a> and my research focusses on developing augmented reality tools to facilitate better surgical planning and training for cardiovascular surgeons. 
	</div>
	<div style="height: 1rem"></div>
	<div>
		I have learnt full-stack technologies, backend tools, cloud computing services, and software development principles through my previous internships at <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/tesla.png">Tesla and <img class="intro-logo" style="width: 19px; padding-bottom: 5px;" src="/images/NCR.png">NCR Corporation.
	</div>
</div>

<!-- <hr class="l-middle home-hr"> -->

<!-- <h2 class="feature-title">Featured <a href="/cv/#publications">Research Publications</a></h2> -->

<!-- <p class="feature-text">
	Latest research for fans of human-computer interaction, data visualization, and machine learning.
</p> -->

<!-- <div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div> -->

<!-- <br>
<h2 class="feature-title">Featured <a href="/dissertation">Dissertation Publications</a></h2> -->

<!-- <p class="feature-text">
	My dissertation contributed interactive interfaces to enable machine learning interpretability at scale and for everyone.
</p> -->

<!-- <div class="cover-wrapper cover-wrapper-1-col l-text">
	{% include dissertation/document.html details=false location=home %}
</div> -->

<!-- <div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedPublications = site.categories.papers | sort: 'feature-order' %}
	{% for feature in sortedPublications %}
		{% if feature.dissertation == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div> -->

<!-- <br>
<h2 class="feature-title">Apple <a href="https://developer.apple.com/design/human-interface-guidelines/">Chart Design Guidelines</a></h2> -->

<!-- <p class="feature-text">
	Guidance and best practices to help designers and developers create the best charts for Apple platforms.
</p> -->

<!-- <div class="cover-wrapper cover-wrapper-2-col l-middle">
	{% for feature in site.data.designs %}
		{% if feature.featured == true %}
			{% include feature.html feature=feature %}
		{% endif %}
	{% endfor %}
</div> -->

<!-- <br>
<h2 class="feature-title">Featured <a href="/cv/#interactive-articles">Interactive Articles</a></h2> -->

<!-- <p class="feature-text">
	Enhanced reading experiences that demonstrate what's possible when dynamic media are effectively combined.
 
</p> -->

<!-- <div class="cover-wrapper cover-wrapper-3-col l-page">
	{% assign sortedArticles = site.data.articles | where: "featured", true %}
	{% assign ia = site.categories.papers | where:"permalink", "papers/interactive-articles" %}

	{% assign feature = sortedArticles[1] %}
	{% include feature.html feature=feature %}

	{% assign feature = sortedArticles[0] %}
	{% include feature.html feature=feature %}

	{% assign feature = ia[0] %}
	{% include feature.html feature=feature %}
</div>

<br>
<h2 class="feature-title"><a href="https://parametric.press/about">Parametric Press</a></h2>

<p class="feature-text">
	A born-digital, experimental magazine dedicated to showcasing the expository power of the web.
</p>

<div class="cover-wrapper cover-wrapper-2-col l-middle">
	{% assign parametric = site.data.articles | where: "parametric-issue", true %}
	{% for feature in parametric %}
		{% include feature.html feature=feature %}
	{% endfor %}
</div> -->

[gt]: http://www.gatech.edu "Georgia Tech"
[cse]: http://cse.gatech.edu "Georgia Tech Computational Science and Engineering"
[coc]: http://www.cc.gatech.edu "Georgia Tech College of Computing"

[cv]: {{ site.url }}/cv
[polo]: http://www.cc.gatech.edu/~dchau/ "Polo Chau"
[alex]: http://va.gatech.edu/endert/ "Alex Endert"
[poloclub]: http://poloclub.gatech.edu "Polo Club of Data Science"
[nstrf]: https://www.nasa.gov/strg/nstrf "NASA Space Technology Research Fellowship"