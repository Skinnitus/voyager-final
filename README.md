# VOYAGER — Travel & Expedition Studio 2.0

Une PWA indépendante, local-first, issue de la comparaison des six archives fournies. L’application s’ouvre vide. Aucun voyage, taux, réservation ou synchronisation fictifs ne sont ajoutés à vos données.

**Pour commencer :** lire `docs/03_GUIDE_HEBERGEMENT_RETOUR_ARRIERE.md`. Déployer sur un NOUVEAU site HTTPS. Garder l’ancienne application et son export JSON. Ne pas remplacer la production.

- `index.html`, `app.js`, `style.css`, `sw.js`, `manifest.webmanifest`, icônes, `_headers` : fichiers d’hébergement à la racine.
- `assets/` : polices locales et visuel de référence réutilisé.
- `licenses/` : licences des polices Inter et Manrope.
- `docs/01_AUDIT_MATRICE_MIGRATION.md` : audit des six sources et contrat de migration.
- `docs/02_RAPPORT_VALIDATION.md` : résultats et limites de validation, à lire avant tout transfert de production.
- `captures/index.html` : galerie de 14 captures réelles + aperçu comparatif.
- `tests/` : données fictives et sorties des tests. Rien dans ce dossier n’est chargé par l’application normale.

Les tests Node du noyau et du service worker passent. Les essais réels du service worker, de l’installation et du coffre dans un navigateur HTTPS et sur Samsung restent à confirmer après hébergement ; l’aperçu de développement est HTTP. Il ne s’agit pas d’une garantie de fonctionnement sur chaque appareil.

Aucune dépendance à installer pour héberger le site. Pas de compilation, de compte serveur ou de clé API. La PWA requiert HTTPS ; ne pas tester via un fichier index.html ouvert directement.
