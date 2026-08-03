# YEDIDIA — site public

Landing page + pages legales du diagnostic d'orientation YEDIDIA.
Site statique servi par GitHub Pages.

| Fichier | Role |
|---|---|
| `index.html` | Landing page |
| `confidentialite.html` | Politique de confidentialite (loi n°2013-450) |
| `mentions-legales.html` | Mentions legales (loi n°2013-546) |
| `.well-known/security.txt` | Contact de signalement de vulnerabilite |
| `robots.txt`, `sitemap.xml` | Indexation |
| `assets/` | Logo, photos, polices auto-hebergees |
| `support.js` | Runtime de rendu |

## A faire avant mise en ligne

1. Deposer les deux polices dans `assets/fonts/` (voir LIRE-MOI.txt).
2. Deployer `inscriptions-yedidia.gs` en Web App, puis renseigner son URL /exec
   dans la propriete `apiUrl` de la page (sinon le formulaire n'enregistre rien).
3. Completer les champs "A completer" des mentions legales (forme juridique,
   RCCM, responsable de la publication).
4. Creer les alias de messagerie : contact@, donnees@, securite@.
5. Passer le domaine derriere Cloudflare pour poser les en-tetes CSP / HSTS /
   X-Frame-Options, impossibles a definir sur GitHub Pages.
