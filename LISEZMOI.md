# Kit de départ : Hugo + Decap CMS + Cloudflare Pages

## À adapter avant la mise en ligne
1. `hugo.toml` : `title` (nom du site) et `baseURL` (adresse du site).
2. `static/admin/config.yml` : `repo` (VOTRE-COMPTE/mon-site), `base_url` et `site_domain`.
3. `static/css/style.css` : la couleur principale (`--couleur`) en haut du fichier.

## Contenu du dossier
- `content/` : les textes du site (modifiés par Decap)
- `layouts/` : les modèles HTML (le design)
- `static/` : CSS, images, et l'administration (`/admin`)
- `functions/api/` : la connexion GitHub pour Decap (projet i40west, licence BSD jointe)

## Réglages Cloudflare Pages
- Framework preset : Hugo
- Commande de build : `hugo`
- Dossier de sortie : `public`
- Variables : `HUGO_VERSION` (ex. 0.170.1, version testée), `GITHUB_CLIENT_ID`, `GITHUB_CLIENT_SECRET`

## Bon à savoir
Une actualité datée dans le futur n'apparaît qu'à partir de cette date (au prochain déploiement).
