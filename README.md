# La Chasse aux Étoiles ⭐

Jeu de révisions (calcul mental, mesures, musique, anglais, français, histoire, logique, géographie) avec étoiles et boutique de récompenses.

Version web autonome, hébergée sur GitHub Pages. Installable sur iPad / téléphone (« Ajouter à l'écran d'accueil ») et utilisable hors ligne.

## Mise en ligne

1. Créer un dépôt GitHub et y pousser le contenu de ce dossier sur la branche `main`.
2. Dans le dépôt : **Settings → Pages → Build and deployment → Source : GitHub Actions**.
3. Le workflow `.github/workflows/pages.yml` publie le site à chaque push. L'adresse s'affiche dans l'onglet **Actions** (en général `https://<utilisateur>.github.io/<dépôt>/`).

## Différences avec la version Claude

- **Progression** : enregistrée dans le navigateur de chaque appareil (localStorage). Pas de synchronisation iPad ↔ téléphone.
- **Atelier photo** : retiré de cette version (aucune photo, aucun appel à Claude).
- **Profils** : « Grand frère » (6ᵉ) et « Petit frère » (CE1), sans prénom.

Après une modification de `index.html`, incrémenter `CACHE` dans `sw.js` (`etoiles-v2`, …) pour que les appareils récupèrent la nouvelle version.
