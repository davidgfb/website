---
title: Projects
layout: single
permalink: /projects/
header:
  overlay_image: /assets/img/a350.jpg
  overlay_filter: 0.5 # same as adding an opacity of 0.5 to a black background
  caption: "Photo credit: [**dfbarrero**](https://www.flickr.com/photos/dfbarrero/)"
  #cta_label: "More Info"
  #cta_url: "https://unsplash.com"
---

<h2 class="bibliography">University projects</h2>

<ol class="bibliography">
{% for project in site.data.projects %}
{% if project.type == "uni" %}
    <li>
         <i>{{ project.name}} </i>. {{ project.desc}}. Participation of {{ project.participants}}. {{ project.years}}.
         <i><a href ="{{ project.link}}">Source Code</a></i>
    </li>
{% endif %}
{% endfor %}
</ol>

<h2 class="bibliography">Personal projects</h2>

<ol class="bibliography">
{% for project in site.data.projects %}
{% if project.type == "personal" %}
    <li>
         <i>{{ project.name}} </i>. {{ project.funding}}. Participation of {{ project.participants}}. PI: {{ project.pi}}. {{project.grant}}. {{ project.years}}.
    </li>
{% endif %}
{% endfor %}
</ol>


