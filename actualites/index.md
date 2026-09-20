---
layout: default
title: "Actualités"
---
<section class="article-header"><div class="container"><span class="category">Bussière Respire</span><h1>Actualités</h1><p class="excerpt">La vie du collectif, ses rendez-vous et ses événements.</p></div></section>
<section class="section section-light"><div class="container"><div class="article-list">{% assign posts = site.posts | where: "category", "Actualités" | sort: "date" | reverse %}{% for post in posts %}<a class="article-link" href="{{ post.url | relative_url }}"><div class="article-date">{{ post.date | date: "%d/%m/%Y" }}</div><div><h3>{{ post.title }}</h3><p>{{ post.excerpt | strip_html }}</p></div></a>{% endfor %}</div></div></section>
