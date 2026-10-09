# Mondial de l'Auto 2026 – Checklist de visite

Application web mobile pour suivre la visite du Mondial de l'Automobile (Paris, Porte de Versailles) : cocher les modèles vus, les noter sur 5 et les commenter, puis agréger les retours de toute l'équipe.

Périmètre : modèles ICE, HEV, PHEV et REEV, plus le stand Renault Group en entier. Données issues du document de préview de l'équipe veille compétiteurs (Competit'R).

## Pour les visiteurs (téléphone)

1. Ouvrir `index.html` via l'adresse de la page (voir « Mise en ligne » ci-dessous).
2. Saisir son nom au premier lancement.
3. Cocher, noter et commenter au fil de la visite. Tout est enregistré **sur le téléphone**, rien n'est envoyé à un serveur.
4. Onglet **Parcours** : plan du site et plans des halls avec le tracé proposé (toucher un plan pour l'agrandir).
5. Onglet **Envoi** : partager le fichier `.json` à l'organisateur (Teams, mail…).

Astuce : ouvrir la page une première fois avec du réseau. Elle fonctionne ensuite hors ligne, et peut être ajoutée à l'écran d'accueil.

## Pour l'organisateur (PC)

Ouvrir `synthese.html`, glisser les fichiers `.json` reçus : nombre de participants, notes moyennes, podium, commentaires par modèle, export CSV.

## Mise en ligne (GitHub Pages)

*Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.*

L'adresse sera `https://<nom-utilisateur>.github.io/<nom-du-depot>/`, et la page de synthèse `…/synthese.html`.

## Fichiers

| Fichier | Rôle |
|---|---|
| `index.html` | Application mobile (données et plans intégrés) |
| `synthese.html` | Page d'agrégation des retours |
| `sw.js`, `manifest.webmanifest`, `icon-*.png` | Mode hors ligne et icône d'écran d'accueil |

## Confidentialité

Aucune donnée n'est collectée : les coches, notes et commentaires restent dans le navigateur de chaque téléphone jusqu'à ce que son propriétaire envoie lui-même son fichier.
