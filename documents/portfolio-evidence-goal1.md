---
title: Goal 1
layout: page
permalink: /goal1
img_url: https://libapps.s3.amazonaws.com/accounts/13366/images/CrownLibraryBanner5.jpg
img_alt: Daytime shot of the Rebecca Crown Library.
---
{% include page-image.html %}

<h2>List of Goal Outcome Artifacts</h2>
{% for artifact in site.artifacts %}
{% if artifact.category == 'goal-1' %}
<h3>{{ artifact.title }}</h3>
<p><img src="{{ artifact.image }}" alt="dominican university logo"/></p>
<p>{{ artifact.content }}</p>
<p>Category: {{ artifact.category }}</p>
{% endif %}
{% endfor %}

<div class="myButton">
<form>
    <input type="BUTTON" value="Back to top" onclick="window.location.href='#top'">
</form>
</div>

<script>
const allPTags = document.querySelectorAll("p");

allPTags.forEach((elem) => {
    if (elem.innerText === "" && elem.childNodes.length === 1 && elem.childNodes[0].tagName === "IMG") {
        elem.parentNode.insertBefore(elem.childNodes[0], elem);
        elem.remove();
    }
});
</script>