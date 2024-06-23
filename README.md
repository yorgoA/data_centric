# Analyse Data-Centric des Ventes E-commerce

## Vue d'ensemble

Ce projet vise à analyser divers ensembles de données liés aux ventes e-commerce, aux avis des clients, à la géolocalisation, et aux données de population pour en tirer des insights business. L'objectif principal est d'identifier des tendances, d'optimiser les stratégies d'expansion du marché, et d'améliorer le ciblage des clients sur la base des analyses de données effectuées.

## Table des Matières

1. [Objectifs du Projet](#objectifs-du-projet)
2. [Ensembles de Données Utilisés](#ensembles-de-données-utilisés)
3. [Préparation et Nettoyage des Données](#préparation-et-nettoyage-des-données)
4. [Analyses Réalisées](#analyses-réalisées)
    - [Distribution des Clients par Ville](#distribution-des-clients-par-ville)
    - [Type de Produit le Plus Vendu par Ville](#type-de-produit-le-plus-vendu-par-ville)
    - [Revenu Total par Ville](#revenu-total-par-ville)
    - [Intégration des Données de Population](#intégration-des-données-de-population)
    - [Calcul des Métriques](#calcul-des-métriques)
    - [Analyse en Composantes Principales (ACP)](#analyse-en-composantes-principales-acp)
5. [Axes Stratégiques Proposés](#axes-stratégiques-proposés)

## Objectifs du Projet

- Analyser les ventes e-commerce pour identifier les tendances et les préférences des clients.
- Optimiser les stratégies d'expansion de marché en utilisant les données démographiques et de vente.
- Améliorer le ciblage des clients par l'analyse des types de produits populaires et les revenus par ville.

## Ensembles de Données Utilisés

- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_customers_dataset.csv`
- `olist_geolocation_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_products_dataset.csv`
- `olist_orders_dataset.csv`
- `olist_sellers_dataset.csv`
- `product_category_name_translation.csv`
- `BRAZIL_CITIES.csv` (pour les données de population des villes)

## Préparation et Nettoyage des Données

1. **Chargement des Données**: 
   - Les données sont chargées depuis des fichiers CSV et JSON à l'aide des fonctions personnalisées `load_csv` et `load_json`.
   - Référence dans le code : **In [5]**

2. **Nettoyage des Données**:
   - Conversion des dates en types datetime pour faciliter les calculs de temps de réponse.
   - Conversion des valeurs numériques pour les paiements en type float.
   - Référence dans le code : **In [7]**

3. **Fusion des Données**:
   - Fusion des différents ensembles de données pour créer une vue complète des ventes.
   - Référence dans le code : **In [8]**

## Analyses Réalisées

### Distribution des Clients par Ville

- **Description**: Analyse de la répartition des clients par ville pour identifier les marchés principaux.
- **Référence dans le code**: **In [6]**

### Type de Produit le Plus Vendu par Ville

- **Description**: Identification des types de produits les plus vendus dans chaque ville pour ajuster l'inventaire et le marketing.
- **Référence dans le code**: **In [11]**

### Revenu Total par Ville

- **Description**: Classement des villes par revenu total pour prioriser les marchés à fort potentiel.
- **Référence dans le code**: **In [12]**

### Intégration des Données de Population

- **Description**: Utilisation des données de population pour enrichir les analyses de vente et évaluer le potentiel du marché.
- **Référence dans le code**: **In [14]**

### Calcul des Métriques

- **Description**: Calcul du CA par client, CA par habitant et la pénétration du marché pour évaluer l'efficacité des ventes.
- **Référence dans le code**: **In [17]**

### Analyse en Composantes Principales (ACP)

- **Description**: Réduction de la dimensionnalité pour identifier les tendances et les regroupements dans les données.
- **Référence dans le code**: **In [24]**

## Axes Stratégiques Proposés

1. **Expansion et Optimisation du Marché**:
   - Cibler les villes avec une forte base de clients pour des campagnes de marketing intensifiées.
   - Explorer les villes avec une faible pénétration de marché mais une population élevée pour des opportunités de croissance.

2. **Gestion des Produits et des Stocks**:
   - Adapter l'inventaire en fonction des préférences locales de produit.
   - Développer des gammes de produits populaires dans des villes spécifiques.

3. **Stratégie de Prix et de Revenus**:
   - Personnaliser la stratégie de prix en fonction du revenu par client et par habitant.
   - Optimiser les offres en fonction du potentiel de revenu total.

4. **Amélioration du Service Client et de la Réponse**:
   - Réduire les délais de réponse pour améliorer la satisfaction client.
   - Mettre en place des programmes de service client proactifs dans les marchés clés.

5. **Segmentation et Ciblage Marketing**:
   - Développer des campagnes marketing segmentées basées sur les composants principaux identifiés.
   - Optimiser le contenu marketing en fonction des préférences des segments identifiés.

6. **Expansions Géographiques et Développement de Marché**:
   - Évaluer les opportunités d'expansion dans les villes avec une faible pénétration mais une population significative.
   - Consolider la position dans les marchés à forte pénétration.

7. **Optimisation de la Chaîne Logistique**:
   - Optimiser la distribution et la logistique en fonction de la densité de clients et de la géographie des ventes.
   - Développer des centres de distribution dans les régions à forte demande pour réduire les délais de livraison.
