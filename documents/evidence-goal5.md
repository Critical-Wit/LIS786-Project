---
title: Goal 5
layout: page
permalink: /goal5
img_url: https://libapps.s3.amazonaws.com/accounts/13366/images/CrownLibraryBanner5.jpg
img_alt: This is some alt text.
footer_link: Back to Top
---
{% include page-image.html %}

<h2>List of Goal Outcome Artifacts</h2>
{% for artifact in site.artifacts %}
{% if artifact.category == 'goal-5' %}
<h3>{{ artifact.title }}</h3>
<p><img src="{{ artifact.image }}" alt="dominican university logo"/></p>
<p>{{ artifact.content }}</p>
<p>Category: {{ artifact.category }}</p>
{% endif %}
{% endfor %}

{{ page.footer_link }}