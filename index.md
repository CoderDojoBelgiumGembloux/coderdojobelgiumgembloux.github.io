---
Title: dojooooo
---

# CoderDojo de Gembloux

Sur ce site vous pouvez retrouver la liste des différentes activités pratiqué durant le dojo.

## Nos 3 derniers dojos

{% for post in site.posts limit:3 %}
* [{{ post.title }}]({{ post.url }}){% endfor %}
* [voir la liste complète](/dojos.md)
