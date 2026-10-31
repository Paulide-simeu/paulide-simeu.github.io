# ITS MARKET

Vitrine commerciale statique pour la vente de spaghettis **Everyday** et **Combino** (500 g) à Douala, Cameroun. Prix : 900 FCFA le paquet. Les commandes se font par WhatsApp.

## Technologies
HTML5, CSS3, icônes SVG intégrées. Aucun JavaScript, aucun framework.

## Structure
```
index.html
mentions-legales.html
404.html
robots.txt
sitemap.xml
css/style.css        styles principaux
css/responsive.css   adaptations tablette / mobile
assets/images/       produits (Everyday, Combino), stock, partage, favicon
assets/icons/        icônes SVG (sources ; intégrées en ligne dans index.html)
```

## Ouvrir le site en local
Double-cliquer sur `index.html`, ou utiliser l'extension « Live Server » de VS Code.
Connexion internet nécessaire pour les polices Google (Inter, Poppins).

## Configuration
- Numéro WhatsApp : `237656648606` (dans les liens `https://wa.me/...` de `index.html`).
- Facebook et TikTok : liens dans le footer. **Instagram : à ajouter** (voir le commentaire dans le footer).
- Les liens WhatsApp ouvrent une conversation avec un message prérempli ; ils n'enregistrent aucune commande.

## Référencement (SEO)
- Adresse prévue : `https://its-market-cameroun.netlify.app/` (hébergement Netlify ; le code est sauvegardé sur GitHub).
- Si l'adresse change (nom de domaine, autre nom de dépôt), mettre à jour : `canonical`, `og:url`, `og:image` et le JSON-LD dans `index.html`, ainsi que `sitemap.xml` et `robots.txt`.
- Après la mise en ligne : valider le site dans Google Search Console et Bing Webmaster Tools, envoyer `sitemap.xml`.

## Sécurité
- Politique CSP stricte dans une balise `<meta>` de chaque page (GitHub Pages n'autorise pas les en-têtes HTTP).
- `_headers` (Netlify, Cloudflare Pages) et `vercel.json` : en-têtes complets, prêts si l'hébergeur change.
- `.nojekyll` : GitHub Pages sert les fichiers tels quels. `SECURITY.md` : contact de signalement.

## Déploiement (GitHub Pages)
Dépôt GitHub > Settings > Pages > Source : branche `main`, dossier `/ (root)`. Tous les chemins sont relatifs, donc compatibles avec un sous-chemin.

## État actuel
Fonctionnel : sidebar en CSS, navigation par ancres, responsive, liens WhatsApp, images et icônes.
À vérifier : mentions légales, délais et zones de livraison à confirmer par le propriétaire.

## Prévu avec JavaScript
Menu interactif, choix des produits et quantités, message WhatsApp construit selon la sélection, validation de formulaire.
