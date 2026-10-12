# INNERSPEECH — Site Quarto (français)

Site public de vulgarisation pour le projet INNERSPEECH (ANR JCJC 2026).

## Prévisualiser en local

1. Installer Quarto : https://quarto.org/docs/get-started/
2. Depuis ce dossier, lancer `quarto preview`.
3. Pour générer le site statique : `quarto render` (résultat dans `_site/`).

## Publier avec GitHub Pages

1. Créer un dépôt GitHub, y déposer les fichiers de ce dossier.
2. **Corriger `website.site-url` dans `_quarto.yml`.**
3. Publier avec `quarto publish gh-pages` (voir https://quarto.org/docs/publishing/github-pages.html). Selon la méthode de publication retenue, la configuration du dépôt GitHub peut varier.
4. Pour un hébergement institutionnel, transférer simplement le contenu généré dans `_site/` sur le serveur.

## Avant la publication publique — points à compléter

- [ ] Remplacer `EXEMPLE` dans l'URL du site de `_quarto.yml`.
- [ ] Remplacer la mention **adresse électronique à renseigner** dans `contact.qmd` par une adresse réellement gérée par l'équipe, et rendre opérationnels les appels à contact.
- [ ] Compléter les mentions légales et celles de l'hébergeur (`mentions.qmd`).
- [ ] Vérifier l'orthographe des noms / institutions et obtenir les accords nécessaires.
- [ ] Revalider le calendrier de l'étude EEG à Aix (avril–mai 2027), de l'étude MEG–IRM 7T à Paris (2028) et du postdoctorat ; ce sont actuellement des prévisions.
- [ ] Préciser les critères, l'indemnisation, la durée et la procédure de recrutement des participant·es après validation des protocoles.
- [ ] Actualiser les publications et annonces au fil du projet.

## Structure

- `index.qmd` : page d'accueil et appels à action.
- `recherche.qmd` : vulgarisation des trois axes.
- `participer.qmd` : études planifiées.
- `recrutements.qmd` : postdoctorat futur, doctorat pourvu.
- `equipe.qmd` : équipe et collaborations.
- `contact.qmd`, `mentions.qmd` : informations pratiques et confidentialité.
- `styles/site.css` : design responsive.
- `assets/*.svg` : illustrations vectorielles originales.

Le site n'utilise pas de services externes de collecte. Les polices web Google Fonts sont chargées à distance dans la feuille CSS ; pour une version sans requête vers Google, supprimer la ligne `@import` de `styles/site.css` et employer des polices système.

**Source scientifique :** proposition complète ANR JCJC 2026 « Mapping the mind's voice: Towards a neurocomputational theory of inner speech », fournie par l'équipe. Les dates de recrutement EEG (avril–mai 2027) et MEG/IRM (2028) proviennent de la demande de réalisation du site, et ne sont pas des dates définitives du protocole.
