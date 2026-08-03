# EverFlow Digital - Site V2

Sources du site public [everflow-digital.com](https://everflow-digital.com/).

## Pages

- `index.html`
- `accompagnement.html`
- `microsoft-intelligent-solutions.html`
- `modern-apps.html`
- `autonomous-intelligence.html`
- `leadflow.html`
- `politique-de-confidentialite.html`

Les routes publiques utilisent des URL propres. Le fichier `.htaccess` assure les
redirections historiques, les en-têtes de sécurité et la compatibilité des ressources.

## Coordonnées officielles

EverFlow Digital<br>
2 Place Jean V<br>
44000 Nantes

Cette adresse doit rester identique dans le pied de page, la page de contact, la politique
de confidentialité et les données structurées `PostalAddress`.

## Invariants critiques

- **Wise** : l'agent Copilot Studio est chargé par la constante `WISE_URL`.
- **Bookings** : la prise de rendez-vous est chargée par la constante `BOOKINGS_URL` et les
  déclencheurs `data-hub-bookings`.
- Les deux services sont présentés dans le widget flottant **EverFlow Hub**.
- Toute modification doit préserver les constantes, le sandbox Wise et les autorisations
  Microsoft de la politique CSP.

Les fichiers de déploiement privés, sauvegardes, checkpoints et identifiants ne font pas
partie du contenu publiable.

## Vérification locale

Servir le dossier par HTTP, puis ajouter `?static=1` à une URL pour désactiver les animations
pendant les captures et tests visuels.
