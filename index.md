---
layout: default
title: Accueil
---

<link rel="stylesheet" href="/assets/style.css">

# Bienvenue sur Mon Blog Minimaliste

Découvrez mes derniers articles ci-dessous :

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%d/%m/%Y" }}
    </li>
  {% endfor %}
</ul>

[À propos]({{ '/about.html' | relative_url }})
