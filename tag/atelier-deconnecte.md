---
layout: tagpage
title: "Atelier déconecté"
tag: atelier-deconnecte
---

Voici les dojos où nous avons effectués des ateliers déconecté :
{% for tag in site.tags %}
  <h3>{{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
