---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<p class="section-note"><sup>*</sup> Equal contribution. See also my <a href="{{ site.author.googlescholar }}">Google Scholar profile</a>.</p>

## Preprints

<ul class="pub-list">
{% for p in site.data.publications %}{% if p.group == "preprint" %}{% include pub-item.html pub=p %}{% endif %}{% endfor %}
</ul>

## Conference Papers

<ul class="pub-list">
{% for p in site.data.publications %}{% if p.group == "conference" %}{% include pub-item.html pub=p %}{% endif %}{% endfor %}
</ul>

## Journal and Workshop Papers

<ul class="pub-list">
{% for p in site.data.publications %}{% if p.group == "other" %}{% include pub-item.html pub=p %}{% endif %}{% endfor %}
</ul>
