# CoderDojo Belgium Gembloux website

Instruction are given in french, because the local dojo is french speaking ;)

## Information sur Github Page

Le site se base sur le moteur jekyll. Les pages sont écrites en markdown.

* [Github Page](https://pages.github.com/)
* [Quickstart jekyll](https://jekyllrb.com/docs/)
* [Markdown summary](https://daringfireball.net/projects/markdown/syntax)
* [Limits](https://help.github.com/en/articles/about-github-pages#usage-limits)
* [Jekyll plugins](https://help.github.com/en/articles/about-github-pages-and-jekyll#plugins)
* [Theme de base](https://github.com/wemake-services/jekyll-theme-hackcss)

## Création de contenu

Pour pouvoir travailler sur le contenu du site, il faut avoir des notions de
* git ou savoir utiliser l'interface de github pour créer des fichier et les modifier.
* markdown

Pour le reste, c'est relativememnt simple, les fichiers `.md` du dossier `src` sont converti par jekyll en html et rendu disponible sur le site web du dojo. Plus d'information sur comment ajouter du contenu est disponible [ici](https://help.github.com/en/articles/adding-content-to-your-github-pages-site-using-jekyll).

### Construction local

#### Avec docker

```
docker run --volume="$PWD:/srv/jekyll" --env BUNDLE_PATH=/srv/jekyll/vendor --rm -ti jekyll/jekyll:3 bundle install
docker run --volume="$PWD:/srv/jekyll" --env BUNDLE_PATH=/srv/jekyll/vendor --rm -ti jekyll/jekyll:3 bundle exec jekyll build
```

#### En utilisant ruby présent sur sa propre machine

```
bundle install
bundle exec jekyll build
```
