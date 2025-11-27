# SquidLandingPage

Landing page statique synchronisée avec les dépôts `squidResearch` et `squidCommunication`.

## Structure

- `index.html` : hero, sections valeur, articles récents (mentions © 2025 SquidResearch™ / RGPD).
- `assets/styles.css` : thème dark basé sur Inter.
- `articles/*.html` : chaque article est une page autonome publiée sur Vercel.
- `bientot.html` : page dédiée aux idées futures (non visibles dans le hero tant qu'elles ne sont pas livrées).

## Synchronisation contenus

1. Déposer les textes/metrics actualisés dans les bases de connaissances (docs & logs).
2. Mettre à jour les articles HTML via script (à créer) ou manuellement.
3. Déployer sur Vercel (`vercel deploy` ou push Git) → la landing se régénère.

> TODO : ajouter `scripts/sync_content.py` pour extraire automatiquement les données des deux dépôts avant build.

## Mentions légales

- Ajouter à chaque nouveau contenu la mention `© 2025 SquidResearch™ – Tous droits réservés`.
- Mettre à jour les liens vers la politique de confidentialité / CGU lorsqu’elles changent côté SquidResearch.
- Les idées futures doivent rester confinées à `bientot.html` jusqu'à leur mise en production.

