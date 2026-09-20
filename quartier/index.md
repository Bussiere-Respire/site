---
layout: default
title: "Notre quartier"
---
<section class="article-header"><div class="container"><span class="category">Bussière Respire</span><h1>Notre quartier</h1><p class="excerpt">Observer les situations concrètes autour de nous.</p></div></section>
<section class="section section-light"><div class="container"><div class="article-list">{% assign posts = site.posts | where: "category", "Notre quartier" | sort: "date" | reverse %}{% for post in posts %}<a class="article-link" href="{{ post.url | relative_url }}"><div class="article-date">{{ post.date | date: "%d/%m/%Y" }}</div><div><h3>{{ post.title }}</h3><p>{{ post.excerpt | strip_html }}</p></div></a>{% endfor %}</div></div></section>
