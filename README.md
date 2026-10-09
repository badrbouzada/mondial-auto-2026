# Mondial de l'Auto 2026 – Checklist de visite

Application web mobile pour suivre la visite du Mondial de l'Automobile (Paris) : cocher les modèles vus, les noter sur 5, les commenter, puis envoyer ses retours par e-mail pour alimenter une synthèse collective.

Périmètre : tous les modèles du document de préview de l'équipe veille compétiteurs (Competit'R), toutes motorisations (ICE, HEV, PHEV, REEV, BEV), avec filtres par motorisation. Le stand Renault Group est toujours affiché.

## Visiteurs (téléphone)
1. Ouvrir l'adresse de l'app, saisir son nom et son équipe (champ libre).
2. Filtrer par motorisation (ICE, HEV, PHEV, REEV, BEV), cocher, noter et commenter. Tout est enregistré sur le téléphone.
3. Onglet **Parcours** : plan du site et plans des halls avec le tracé proposé.
4. Onglet **Envoi** : un bouton ouvre l'e-mail pré-rempli et adressé. Il suffit d'appuyer sur Envoyer.

Ouvrir l'app une première fois avec du réseau : elle fonctionne ensuite hors ligne.

## Organisateur
Les e-mails reçus alimentent une table Excel (flux Power Automate). `synthese.html` agrège cette table : moyennes, commentaires, filtres par motorisation et par équipe.

## Configuration
Le destinataire des e-mails est défini dans `config.js`. Il peut être remplacé par lien avec `?to=adresse@exemple.com`.

## Fichiers
| Fichier | Rôle |
|---|---|
| `index.html` | Application mobile (catalogue et plans intégrés) |
| `synthese.html` | Page d'agrégation des retours |
| `config.js` | Destinataire des retours |
| `sw.js`, `manifest.webmanifest`, `icon-*.png` | Mode hors ligne et icône d'écran d'accueil |

Aucune donnée n'est collectée par le site : les retours restent sur le téléphone jusqu'à l'envoi volontaire de l'e-mail.
