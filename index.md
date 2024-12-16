---
layout: default
title: Accueil
---

# Bienvenue sur Mon Blog Minimaliste

Découvrez mes derniers articles :

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> - {{ post.date | date: "%d/%m/%Y" }}
    </li>
  {% endfor %}
</ul>