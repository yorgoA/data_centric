# Analyse de la rentabilité des villes et ACP

## 1. Réponse à la problématique : "Est-ce que ce sont les plus grandes villes qui sont les plus rentables ?"

### 1.1. Calcul du revenu total par ville

Nous avons calculé le revenu total généré par chaque ville à partir des données de paiement. Cela a été effectué dans la section **"Calcul du revenu total par ville"** de notre script.

![Graphique du Revenu Total par Ville](/./graphs/total_revenue_by_city.png)

### 1.2. Mise en relation avec la population

Pour analyser la rentabilité en fonction de la taille des villes, nous avons fusionné les données de revenu avec les données de population dans la section **"Fusion des Données pour Analyse"**.

### 1.3. Visualisation et comparaison du revenu total par ville

Le graphique ci-dessus, généré dans la section **"Visualisation du Revenu Total par Ville"**, montre les villes avec le revenu total le plus élevé.

### 1.4. Calcul du chiffre d'affaires (CA) par client et par habitant

Pour une comparaison plus équilibrée, nous avons calculé le CA par client et par habitant dans la section **"Calcul des Indicateurs Clés"** de notre code.

Voici le graphique montrant les 20 principales villes selon le CA par habitant, généré dans la section **"Visualisation des Villes Principales par CA par Habitant"** :

![Graphique des 20 principales villes selon le CA par habitant](/./graphs/ca_per_capita.png)

## 2. Analyse de l'analyse en composantes principales (ACP)

L'ACP a été utilisée pour réduire la dimensionnalité des données tout en conservant les principales variations entre les observations. Cette analyse est détaillée dans la section **"Analyse en Composantes Principales (ACP)"**.

### 2.1. préparation des données pour l'ACP

Les colonnes numériques pertinentes ont été sélectionnées et standardisées dans la section **"Préparation des Données pour l'ACP"**.

### 2.2. Application de l'ACP

L'ACP a été appliquée pour réduire les données à deux dimensions principales. Le graphique de la distribution des données selon les deux premières composantes principales est généré dans la section **"Application de l'ACP"**.

![Graphique de l'ACP](/./graphs/pca_scatterplot.png)

### 2.3. Variance expliquée par les composantes principales

La proportion de la variance totale capturée par chaque composante principale a été calculée et visualisée dans la section **"Variance Expliquée par les Composantes Principales"**.

![Variance Expliquée](/./graphs/variance.png)

### 2.4. Charges des composantes principales

Les charges montrent l'influence de chaque variable d'origine sur les composantes principales. Cela a été visualisé dans la section **"Charges des Composantes Principales"**.

![Charges des Composantes](/./graphs/pca_loading.png)

### Conclusion de l'ACP

Les résultats de l'ACP montrent que :
- La première composante principale (PC1) capture environ 50% de la variance totale.
- La deuxième composante principale (PC2) capture environ 30% de la variance totale.
- Les charges des composantes indiquent que les variables `total_revenue`, `num_clients`, et `IBGE_RES_POP` ont des charges élevées pour PC1, tandis que `CA_per_Client` et `CA_per_Capita` ont des charges significatives pour PC2.

Ces résultats montrent que les grandes villes avec une population importante tendent à avoir un revenu total plus élevé, mais la rentabilité par habitant ou par client peut varier. Les analyses visuelles et les métriques calculées fournissent une compréhension claire de la relation entre la taille de la ville et sa rentabilité.

## Références

- **Data Sources:** Les données utilisées dans cette analyse proviennent des datasets suivants :
  - `olist_order_payments_dataset.csv`
  - `olist_order_reviews_dataset.csv`
  - `olist_customers_dataset.csv`
  - `olist_geolocation_dataset.csv`
  - `olist_order_items_dataset.csv`
  - `olist_products_dataset.csv`
  - `olist_orders_dataset.csv`
  - `olist_sellers_dataset.csv`
  - `product_category_name_translation.csv`
  - `BRAZIL_CITIES.csv`

