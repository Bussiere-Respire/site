---
layout: default
title: "Accueil"
---
<section class="hero"><div class="container"><h1>Un quartier qui respire.</h1><p>Comprendre notre ville, imaginer son avenir.</p><a class="hero-link" href="#commencer">Commencer ici : comprendre les enjeux ↓</a></div></section>
<section class="section" id="commencer"><div class="container"><div class="intro-box"><h2>Vous découvrez le site ? Commencez par comprendre.</h2><p>Avant de parler de solutions, prenons le temps de regarder ce qui se passe dans nos rues : déplacements, bruit, air, climat, santé et place accordée aux différents usages.</p></div></div></section>
<section class="section section-light"><div class="container"><div class="section-title"><h2>Une petite bibliothèque pour comprendre</h2><p>Des articles courts, accessibles et documentés pour avancer progressivement.</p></div><div class="cards">
<a class="card" href="{{ '/comprendre/' | relative_url }}"><span class="card-number">01</span><h3>Comprendre</h3><p>Climat, ville, déplacements, pollution et santé.</p></a>
<a class="card" href="{{ '/quartier/' | relative_url }}"><span class="card-number">02</span><h3>Notre quartier</h3><p>Observer les rues et les usages concrets.</p></a>
<a class="card" href="{{ '/agir/' | relative_url }}"><span class="card-number">03</span><h3>Agir</h3><p>Des pistes pour rendre les déplacements quotidiens plus simples et plus agréables.</p></a>
<a class="card" href="{{ '/nous-rejoindre/' | relative_url }}"><span class="card-number">04</span><h3>Qui sommes-nous ?</h3><p>Découvrir le collectif et participer.</p></a>
</div></div></section>
<section class="section"><div class="container"><div class="section-title"><h2>La vie du collectif</h2><p>Les événements et rendez-vous sont relayés ici.</p></div><div class="article-list">{% assign news = site.posts | where: "category", "Actualités" | sort: "date" | reverse %}{% for post in news limit:3 %}<a class="article-link" href="{{ post.url | relative_url }}"><div class="article-date">{{ post.date | date: "%d/%m/%Y" }}</div><div><h3>{{ post.title }}</h3><p>{{ post.excerpt | strip_html }}</p></div></a>{% endfor %}</div><p class="more"><a href="{{ '/actualites/' | relative_url }}">Voir toutes les actualités →</a></p></div></section>
<section class="newsletter"><div class="container"><div class="newsletter-inner"><h2>Recevoir les nouvelles du collectif</h2><p>Une adresse e-mail suffit pour recevoir les informations importantes.</p><form action="#" method="post"><label for="email" class="sr-only">Adresse e-mail</label><input id="email" name="email" type="email" placeholder="Votre adresse e-mail" required><button class="button" type="submit">S'inscrire</button></form></div></div></section>
