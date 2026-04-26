# Holiaē Cockpit

PWA statique pour piloter les données business HOLIAĒ depuis Google Sheets.

## Configuration

1. Rends le Google Sheet lisible par lien en lecture seule.
2. Crée une clé API Google Sheets dans Google Cloud.
3. Ouvre `index.html`.
4. Remplace :

```js
const API_KEY = "TA_CLE_ICI";
```

par ta clé.

## Déploiement GitHub Pages

1. Crée un repo GitHub.
2. Envoie les fichiers du dossier `holiae_cockpit_pwa`.
3. Va dans `Settings > Pages`.
4. Source : branche `main`, dossier racine.
5. Ouvre l'URL GitHub Pages sur iPhone.
6. Safari > Partager > Ajouter à l'écran d'accueil.

## Données lues

- `Shopify_Daily`
- `GA4_Channel`
- `GoogleAds_Campaigns`
- `GoogleAds_SearchTerms`
- `GSC_Pages`
- `GSC_Queries`
- `Klaviyo`
- `Objectifs` si disponible

## Limites v1

Le funnel est partiel tant que `Shopify_Daily` ne contient pas `Sessions`, `Product page sessions`, `Add to cart` et `Checkout started`.
Clarity et Meta Ads ne sont pas branchés dans cette v1.
