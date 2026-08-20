# felicitas-strahm

Site one-page de Felicitas Christine Strahm – Seelenzentriertes Coaching & Tao Tantric Arts.

`index.html` porte le CSS et le JavaScript en ligne. Les images sont des
fichiers : `frames/01.jpg` à `frames/35.jpg` pour l'animation du hero,
`portrait.jpg`, et `share.jpg` pour l'aperçu des liens partagés. Seul le logo
reste en data URI, pour qu'il s'affiche sans attendre une requête. Aucune
dépendance externe en dehors des Google Fonts.

## Déploiement

Le workflow `.github/workflows/deploy-pages.yml` publie la racine du dépôt sur
GitHub Pages à chaque push sur `main` ou `claude/index-html-github-pages-m7nopa`,
et peut aussi être lancé manuellement (« Run workflow »).

Étape unique à faire une fois dans l'interface GitHub :
**Settings → Pages → Build and deployment → Source : GitHub Actions.**
Le jeton d'Actions n'a pas le droit de créer le site Pages lui-même ; une fois la
source sélectionnée, relancer le workflow suffit à publier.

URL du site après publication :
<https://antoinelecoquierre.github.io/felicitas-strahm/>

## Développement local

Ouvrir `index.html` dans un navigateur, ou servir le dossier :

```sh
python3 -m http.server 8000
```
