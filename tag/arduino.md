---
layout: tagpage
title: "Arduino"
tag: arduino
---

Les arduino sont des petites cartes électroniques prévues pour facilité l'apprentissage et l'expérimentation de l'électronique. Il s'agit donc d'outils idéal pour ceux qui désires expérimenté.

Plus d'information sur [wikipedia](https://fr.wikipedia.org/wiki/Arduino).

Voici les dojos où nous avons utilisé des arduinos :
{% for tag in site.tags %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
