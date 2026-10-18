# VKT Item Pin

[English](../README.md) | [中文](README_zh.md) | [Español](README_es.md) | [Deutsch](README_de.md) | [日本語](README_ja.md) | Français

Une extension de navigateur pour la recherche shopping : capturez des fiches produits d'un simple survol. Titre, prix, lien, modèle, site et date sont enregistrés dans une bibliothèque locale, avec suivi automatique de l'historique des prix.

> Basé sur Chromium · Manifest V3 · Autorisations minimales · Aucun tracking · 100 % local

---

## Pourquoi VKT Item Pin ?

Comparer des produits entre sites marchands, c'est souvent des dizaines d'onglets ouverts et du copier-coller dans un tableur. VKT Item Pin vous permet de survoler un produit, de cliquer sur **Pin** et de construire une bibliothèque suivie dans le temps, directement dans votre navigateur.

| Avantage | Détail |
|----------|--------|
| 🎯 **Capture au survol** | Survolez un produit et cliquez sur Pin — titre, prix, lien, modèle, site et date extraits automatiquement |
| 🔁 **Prix relevé automatiquement** | Rouvrez une fiche produit déjà épinglée : le prix est enregistré sans second clic |
| 🔔 **Alerte de prix locale** | Fixez un prix cible par produit : la première visite qui l'atteint ou passe en dessous déclenche une notification système, sans serveur ni e-mail |
| 📈 **Historique des prix** | Chaque capture, manuelle ou automatique, ajoute un point et construit le graphique de tendance |
| 🛒 **24 sites préconfigurés** | Sélecteurs ajustés pour Amazon, eBay, Etsy, Walmart, AliExpress, Temu et plus — plus un moteur universel (JSON-LD / OG / sélecteurs génériques) pour toutes les autres boutiques |
| 🏷 **Notes et étiquettes** | Notez la raison (« attendre le Black Friday ») et classez avec jusqu'à 10 étiquettes par produit, toutes cherchables |
| 🖼️ **Vignettes** | L'image du produit est enregistrée avec chaque fiche |
| 🔒 **Confidentialité d'abord** | Toutes les données restent dans votre navigateur via `chrome.storage.local`. Rien n'est envoyé en ligne |

---

## Fonctionnalités

### 🆓 Gratuit

| Fonctionnalité | Description |
|----------------|-------------|
| 🎯 **Capture en un clic** | Épinglez n'importe quel produit, sur une fiche produit ou dans une grille de résultats |
| 📋 **Aperçu et sélection** | Modifiez les champs avant d'enregistrer ; le mode « Choisir » remplit un champ en cliquant sur un élément de la page |
| 🔁 **Historique automatique** | Rouvrir un produit épinglé relève le prix en arrière-plan : un point par jour maximum |
| 🔔 **Alerte de prix cible** | Fixez un prix cible par produit ; la capture qui l'atteint pour la première fois affiche une notification système (100 % locale) |
| 📈 **Historique des prix** | Recaptures illimitées sur les produits suivis, avec graphique de tendance par article |
| 🏷 **Notes et étiquettes** | Une note libre et jusqu'à 10 étiquettes par produit ; les deux sont cherchables et filtrables |
| 📊 **Statistiques** | Bandeau récapitulatif : nombre de baisses sur 30 jours et valeur totale d'une bibliothèque en une seule devise |
| 🧭 **Comparer ailleurs** | Un clic pour rechercher le même titre sur Google Shopping, eBay ou Amazon |
| ✏️ **Modifier les fiches** | Corrigez titres et modèles, corrigez ou supprimez les points de prix erronés, modifiez notes, étiquettes et prix cible |
| 💾 **Sauvegarde JSON** | Exportez / importez une sauvegarde complète de votre bibliothèque (hors ligne), notes, étiquettes et prix cible inclus |
| 🧮 **Moniteur de stockage** | Affiche l'utilisation réelle et alerte avant saturation |
| 🌍 **6 langues** | Anglais, chinois, japonais, espagnol, allemand, français |

### ⭐ Pro (licence requise)

| Fonctionnalité | Description |
|----------------|-------------|
| ♾️ **Produits illimités** | Le plan gratuit couvre 50 produits ; Pro supprime la limite (les recaptures ne comptent jamais) |
| 🔍 **Filtres avancés** | Filtrez par site, étiquette, période et fourchette de prix |
| 📤 **Export CSV** | Format long (une ligne par point de prix, avec BOM, compatible Excel) incluant notes, étiquettes et prix cible |
| 📊 **Comparaison multi-produits** | Superposez l'historique de prix de 6 produits dans un même graphique |

---

## Sites pris en charge

**Préréglages manuels (24) :** Amazon (toutes marketplaces), eBay, Etsy, Walmart, Target, AliExpress, Temu, Best Buy, Home Depot, Lowe's, Newegg, Wayfair, Mercari, Shopee, Lazada, Rakuten, SHEIN, Alibaba.com / 1688, DHgate, TikTok Shop, bol.com, Allegro, Otto.de, Cdiscount…

**Tout le reste** (Shopify / WooCommerce / boutiques indépendantes) est couvert par le moteur universel : données structurées JSON-LD → balises Open Graph → sélecteurs génériques → expressions régulières → mode de sélection manuelle.

---

## Navigateurs pris en charge

| Navigateur | Statut |
|------------|--------|
| Google Chrome | ✅ Entièrement pris en charge |
| Microsoft Edge | ✅ Entièrement pris en charge |
| Autres navigateurs Chromium | ✅ Devrait fonctionner |

---

## Installation

1. Ouvrez la page des extensions : **Chrome** `chrome://extensions/` · **Edge** `edge://extensions/`
2. Activez le **Mode développeur** (interrupteur en haut à droite)
3. Cliquez sur **Charger l'extension non empaquetée** et sélectionnez le dossier `vkt-item-pin`
4. Survolez n'importe quel produit et cliquez sur le bouton 📌 Pin

---

## Utilisation

### Capturer un produit

1. Survolez un produit (fiche produit **ou** grille de résultats) — le bouton 📌 apparaît
2. Cliquez : un panneau latéral s'ouvre avec le titre, le prix, le lien, le modèle, le site et la date extraits
3. Corrigez ce qu'il faut, utilisez **Choisir** pour compléter un champ manquant, puis cliquez sur **Enregistrer**

### Suivre les prix

- Rouvrez simplement une fiche déjà enregistrée : le prix est relevé automatiquement, un point par jour maximum (les produits suivis ne consomment jamais le quota gratuit)
- Définissez un **prix cible** dans le tableau de bord : quand une visite amène le prix à ce niveau ou en dessous, une notification système s'affiche, une seule fois par franchissement et sans répétition
- Ouvrez le tableau de bord pour le graphique de tendance et le bilan des baisses sur 30 jours, ou utilisez **Comparer** (Pro) pour superposer plusieurs produits
- Utilisez **note** et **étiquettes** pour garder en tête pourquoi le produit vaut l'attente

### Sauvegarde

- Le pied du tableau de bord propose **Sauvegarde JSON** / **Importer** — recommandé régulièrement, car les données ne vivent que dans votre navigateur

---

## Confidentialité

- `storage` — Enregistre votre bibliothèque localement. Aucun contenu de page ne quitte votre navigateur.
- `scripting` + `activeTab` — Injectent le bouton Pin / extraient les champs uniquement pendant votre interaction.
- `notifications` — Utilisée uniquement pour les alertes locales de prix cible ; rien n'est envoyé nulle part.
- `<all_urls>` — Permet de fonctionner sur tous les sites marchands. Ne lit ni n'envoie jamais de contenu en arrière-plan.
- Aucun tracking, aucune analytics. La seule requête réseau est l'activation/validation de la licence Pro.

---

## Licence

Copyright © 2026 VKT Item Pin. Tous droits réservés.

---

## ❤️ Soutenir

Si VKT Item Pin vous est utile, pensez à soutenir le projet !

**[👉 Obtenir une clé de licence](https://www.annmax1983.com/checkout.html?plugin=itempin)** · [GitHub](https://github.com/annmax1983/ItemPin) · [Site officiel](https://www.annmax1983.com/extensions/itempin)
