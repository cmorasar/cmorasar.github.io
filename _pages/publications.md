---
layout: archive
title: "Publications & Talks"
permalink: /publications-talks/
author_profile: true
---

<h2>Publications</h2>

{% if site.author.googlescholar %}
<p>You can also find my publications on <a href="{{ site.author.googlescholar }}">my Google Scholar profile</a>.</p>
{% endif %}

{% assign pub_years = site.data.publications | map: "year" | uniq | sort | reverse %}
{% for y in pub_years %}
<h3 class="entry-year">{{ y }}</h3>
<ul class="entry-list">
  {% for p in site.data.publications %}{% if p.year == y %}
  <li class="entry">
    <p class="entry__title">
      {{ p.title }}
    </p>
    {% if p.award %}<p class="entry__award-row"><span class="entry__award">{{ p.award }}</span></p>{% endif %}
    <p class="entry__authors">{{ p.authors | replace: "Carlos Mora", "<strong>Carlos Mora</strong>" }}</p>
    {% if p.note %}<p class="entry__note">*{{ p.note }}</p>{% endif %}
    <p class="entry__meta">{{ p.venue }}{% for l in p.links %}<span class="entry__sep">&middot;</span><a href="{{ l.url }}">{{ l.label }}</a>{% endfor %}</p>
  </li>
  {% endif %}{% endfor %}
</ul>
{% endfor %}

<h2>Talks</h2>

{% assign talk_years = site.data.talks | map: "year" | uniq | sort | reverse %}
{% for y in talk_years %}
<h3 class="entry-year">{{ y }}</h3>
<ul class="entry-list">
  {% for t in site.data.talks %}{% if t.year == y %}
  <li class="entry">
    <p class="entry__title">{{ t.title }}</p>
    <p class="entry__meta">{{ t.venue }}{% for l in t.links %}<span class="entry__sep">&middot;</span><a href="{{ l.url }}">{{ l.label }}</a>{% endfor %}</p>
  </li>
  {% endif %}{% endfor %}
</ul>
{% endfor %}
