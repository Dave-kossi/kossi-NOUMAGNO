# Kossi NOUMAGNO
###  Junior Data Scientist | AI Engineer | Mathematical Engineer (M2)
**Specialized in Mathematical Modeling, Data Science & Machine Learning**

<p align="center">
<a href="https://www.linkedin.com/in/kossi-noumagno">
  <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
<a href="https://github.com/Dave-kossi">
  <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white"/>
</a>
<a href="mailto:noumagnokossi0@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
</p>

📍 **Brunstatt (France)** | 📞 **+33 7 45 97 43 82**

---

## 🔬 Profil
Étudiant en Master 2 Ingénierie Mathématique & Data Science, spécialisé en analyse de données, modélisation mathématique et automatisation. J'ai développé une solide expérience dans la conception de solutions data orientées décisionnel (transition énergétique, maintenance prédictive, analyse de données en temps réel). Je suis compétent en structuration, nettoyage et exploitation de bases de données complexes pour améliorer la performance opérationnelle. Je recherche activement un stage de fin d'études en data science et ML dans les secteurs de l'énergie ou de l'industrie à partir de mars 2027.

---

## 🛠️ Stack Technique

### 💻 Langages
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)

---

### 🧠 Data Science & Machine Learning
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch)

🧩 NumPy | Modélisation mathématique 

---

### 🗄️ Data Engineering & Bases de données
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb)
![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)

🧩 SQL | NoSQL | API REST | Data Cleaning | Feature Engineering | Pipelines ETL

---

### 📈 Data Visualisation & BI
![PowerBI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=microsoftpowerbi)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit)

🧩 Tableau | Matplotlib | Seaborn | Data Storytelling

---

### ⚙️ Outils & Cloud
![Git](https://img.shields.io/badge/Git-F05033?style=for-the-badge&logo=git)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle)
![Google Cloud](https://img.shields.io/badge/GoogleCloud-4285F4?style=for-the-badge&logo=google-cloud)

🧩 Hugging Face | Excel / Google Sheets | GitHub

---

## 🎓 Projets Universitaires & Recherche Académique

### 🌀 PINNs pour Systèmes Dynamiques Chaotiques (Master 1)
👉 [Lien vers le dépôt du projet](https://github.com/Dave-kossi/PINNs-for-chaotic-system)

*   **Objectif :** Résoudre et reconstruire le système chaotique hautement non linéaire de Lorenz ($\sigma = 10, \rho = 28, \beta = 8/3$) à l'aide de réseaux de neurones informés par la physique (**PINNs**). L'étude compare une architecture standard à une version améliorée par des plongements de Fourier pour atténuer le biais spectral du MLP et capturer les hautes fréquences dynamiques.
*   **Méthodologie & Architecture :** MLP à 4 couches cachées (256 neurones, activation `tanh`) entraîné sur 500 points de référence RK45 et 1000 points de collocation. Implémentation d'un encodage sinusoïdal multicouche pour les fréquences $f_k \in \{1,2,4,8,16,32\}$. La fonction de perte combine la supervision des données et les résidus physiques de l'EDO :
$$\mathcal{L} = \lambda_{data}\mathcal{L}_{data} + \lambda_{ODE}\mathcal{L}_{ODE}$$
*   **Stratégie d'Optimisation :** Stratégie de *curriculum learning* en trois étapes : pré-entraînement supervisé, introduction progressive des contraintes de l'EDO, et raffinement final via l'optimiseur **L-BFGS**.
*   **Résultats Comparatifs (Erreur Globale $L_2$) :**
    *   *Problème Direct (Prédiction de l'état complet) :* Standard PINN = 0.105 vs **PINN-Fourier = 0.061**
    *   *Problèmes Inverses (Observabilité partielle via un seul capteur) :* L'architecture PINN-Fourier surpasse systématiquement le modèle standard, identifiant la variable $y(t)$ comme la plus informative pour reconstruire l'attracteur étrange (Erreur réduite à **0.197**).
*   **Applications Métier :** Jumeaux numériques en ingénierie, assimilation de données en météorologie, réduction du nombre de capteurs physiques requis pour la surveillance industrielle active.
---

### 🎲 Modélisation Stochastique : Chaînes de Markov appliquées au Jeu de Kruskal (L3)
*Projet de Fin de Cycle – Mathématiques Appliquées*

#### 📋 Contexte & Objectifs
Formaliser et démontrer mathématiquement le principe de couplage de Kruskal (Kruskal's Count) — un phénomène probabiliste où des trajectoires de calcul démarrant de points initiaux différents convergent inévitablement vers un état absorbant commun (effet d'absorption stochastique).

#### 🛠️ Approche Théorique & Algorithmique
* **Modélisation Stochastique** : Définition formelle de l'espace des états (valeurs de cartes et longueurs de sauts) et construction de la **matrice de transition stochastique** $P$.
* **Analyse Asymptotique** : Étude approfondie des propriétés de la chaîne (irréductibilité, apériodicité) et calcul analytique des probabilités d'absorption pour quantifier le taux de réussite théorique du couplage (généralement $> 85\%$).
* **Simulation Numérique** : Développement de scripts de simulation (Python/R) pour valider empiriquement la vitesse de convergence de la loi de probabilité vers la distribution stationnaire théorique.

#### 📈 Résultats & Impact
Démonstration rigoureuse de la convergence théorique complétée par une validation empirique robuste. Ce projet valide des compétences avancées en calcul matriciel et en modélisation de processus stochastiques.

---

##  Projets Data Science & Machine Learning (Personnels & R&D)

---

### 🛡️ Détection de Fraude Bancaire Optimisée
👉 [Lien vers le dépôt du projet](https://github.com/Dave-kossi/bank-transaction-fraud-detection)

*   **Objectif :** Concevoir une architecture de Machine Learning capable de détecter les transactions frauduleuses omnicanales en temps réel, minimisant les pertes financières tout en préservant l'expérience client (limitation des faux positifs).
*   **Méthodologie & Stack :** Feature engineering comportemental, gestion du fort déséquilibre de classes (50k+ lignes) et benchmarking d'algorithmes (*Logistic Regression, Random Forest, XGBoost, LightGBM*). Validation robuste par *5-Fold Cross-Validation*.
*   **Arbitrage Technique (Précision/Rappel) :** Sélection de **LightGBM** comme modèle final. Il offre le meilleur équilibre industriel avec une **Précision chirurgicale de 99.7%** (pour éviter de bloquer des clients légitimes) et un **Rappel de 62.0%** (capturant efficacement les fraudes complexes là où les règles de sécurité classiques comme l'OTP ou le PIN échouent).
*   **Interprétabilité (XAI) :** Le modèle fonde ses prédictions sur le croisement de signaux faibles : le ratio montant/solde du compte (`Transaction_Amount` vs `Account_Balance`), la déviation par rapport à la moyenne hebdomadaire (`Avg_Transaction_Amount_7d`) et l'incohérence géographique (`Transaction_Distance`).
*   **Impact Économique :** Coût moyen d'une fraude non détectée estimé à **3,10 €**. Sur une simulation de 10 000 transactions, le déploiement de LightGBM **réduit les pertes financières de 62%** (coût chutant de 310,00 € à 117,80 €), maximisant directement le ROI opérationnel.
  
---

### ⚡ Europa Énergie – Intelligence Décisionnelle & Modélisation Prospective
🌐 [🔥 Voir la démo live](https://euenergyconsomption-dmjfgddsphmd4ydjqlscgk.streamlit.app/)

#### 📋 Contexte & Objectifs
Concevoir un outil d'intelligence décisionnelle pour analyser la transition énergétique en Europe, évaluer la performance des pays (renouvelables, intensité carbone, vitesse de transition) et simuler des scénarios prospectifs à horizon 2050, à partir des données ouvertes Our World in Data (OWID Energy).

#### 🛠️ Approche Technique & Méthodologie
* **Stack** : Python, Pandas, NumPy, Plotly, Streamlit, SciPy.
* **Clustering & Profiling** : Classification non supervisée (K-Means / Hiérarchique) sur des critères multicritères normalisés (intensité carbone, part EnR, dépendance fossile) et modélisation dynamique des trajectoires de migration des pays depuis 2010.
* **Modélisation Prospective** : Développement de modèles de projection statistique jusqu'en 2050 (Tendances linéaires vs Scénarios Objectif Zéro Net) avec calcul d'**intervalles de confiance à 95%** via `SciPy`.
* **Calculs Économétriques** : Implémentation du Taux de Croissance Annuel Composé (**TCAC / CAGR**) pour les énergies de transition (solaire/éolien) et mesure de la vitesse de décarbonation glissante sur 10 ans.

#### 📈 Résultats & Impact Métier
Déploiement d'une application d'intelligence décisionnelle interactive (Streamlit) calculant un score d'ambition national unique et générant des recommandations stratégiques automatisées pour l'allocation des fonds de transition.

---

### ⚙️ Maintenance Prédictive Industrielle & Analyse de Survie
👉 [Code GitHub](https://github.com/Dave-kossi/Predictive-Maintenance-in-industry)

#### 📋 Contexte & Objectifs
Estimer la probabilité de panne des machines et réduire les coûts opérationnels consécutifs à un arrêt d'une machine en production au sein de chaînes industrielles complexes.

#### 🛠️ Approche Technique & Méthodologie
* **Stack** : Python, Lifelines, Plotly, Streamlit.
* **Modélisation Statistique** : Utilisation de l'**estimateur non-paramétrique de Kaplan-Meier** pour modéliser le cycle de vie des machines.
* **Analyse des Défaillances** : Étude fine des fonctions de survie et calcul des taux de défaillance instantanés (*Hazard Rate*) pour estimer la durée de vie résiduelle utile (RUL - *Remaining Useful Life*).

#### 📈 Résultats & Impact Métier
Mise en place d'un cadre prédictif opérationnel permettant de planifier les interventions de maintenance corrective juste avant la phase critique d'usure statistique, optimisant la chaîne logistique de production.

---

### 🚲 Collecte et Analyse de Données Temps Réel : Vélostation de Mulhouse
🌐 [🔥 Voir la démo live](https://biketrack-jq9uepdtfbywzdccc5tvim.streamlit.app/)

#### 📋 Contexte & Objectifs
Automatiser la collecte de données des stations de vélos en libre-service de l'agglomération mulhousienne (m2A), analyser les taux d'occupation et construire un jeu de données historique complet pour entraîner des modèles prédictifs de disponibilité.

#### 🛠️ Approche Technique & Méthodologie
* **Stack** : Python, Streamlit, Pandas, Data Engineering, Time Series.
* **Data Engineering Temps Réel** : Développement d'un pipeline automatisé de collecte et de nettoyage de données (ETL) branché directement sur l'API publique de la m2A.
* **Analyse de Séries Temporelles** : Décompositions saisonnières des historiques de charge et modélisation des flux de pointes (matin/soir, jours ouvrés/week-ends).

#### 📈 Résultats & Impact Métier
Déploiement d'une application Streamlit de monitoring en temps réel, posant les fondations de l'infrastructure de données nécessaire à l'optimisation des tournées de régulation logistique.

---

### 🏥 Insurance Risk Intelligence & Predictive Pricing
🌐 [🔥 Voir la démo live](https://predictive-analysis-g7zjxrbuf79tfb3aolobma.streamlit.app/) | 👉 [Code GitHub](https://github.com/Dave-kossi/healthcare-cost-analysis)

#### 📋 Contexte & Objectifs
Transformer des données démographiques et comportementales (Dataset *Insurance* de Kaggle) en une plateforme d'aide à la décision (BI) et un moteur de tarification dynamique (*Smart Pricing*) à destination des compagnies d'assurance.

#### 🛠️ Approche Technique & Méthodologie
* **Modélisation Prédictive** : Implémentation d'une Régression Linéaire Multiple avec validation croisée pour l'estimation en temps réel des charges médicales individuelles.
* **Algorithme Actuariel "Risk-Pulse"** : Conception d'un système de scoring propriétaire (échelle de 0 à 10) formalisant l'impact non-linéaire des facteurs de risque combinés (ex: l'interaction tabagisme + obésité avec un BMI $\ge 30$ multiplie les charges par **3.8x**).

#### 📈 Résultats & Impact Métier
Traduction instantanée des scores de risque en stratégies tarifaires directes (de -20% de bonus pour profils sains à +35% de surprime critique), optimisant directement le ratio de sinistralité (*Loss Ratio*) de l'assureur.

---

### 🛒 Analyse Interactive des Ventes & Segmentation RFM (E-Commerce)
🌐 [🔥 Voir la démo live](https://onlineretailproject-n4u86pch6tfkxqdhtaceco.streamlit.app/) | 👉 [Code GitHub](https://github.com/Dave-kossi/online-retail-analysis.git)

#### 📋 Contexte & Objectifs
Valoriser un volume massif de données transactionnelles (+500 000 lignes, dataset *Online Retail* de l'UCI) pour en extraire des leviers de croissance commerciale et optimiser les campagnes marketing de fidélisation.

#### 🛠️ Approche Technique & Méthodologie
* **Data Engineering & Nettoyage** : Conception d'un pipeline ETL robuste (gestion stricte des transactions annulées, traitement des valeurs aberrantes de quantité via la méthode des écarts interquartiles $IQR$).
* **Segmentation Comportementale (RFM)** : Calcul dynamique des scores de **Récence, Fréquence et Montant** par client, suivi d'un regroupement algorithmique en segments exploitables (*Champions, À risque*).

#### 📈 Résultats & Impact Métier
Déploiement d'une application de Business Intelligence (Streamlit/Plotly) permettant à une direction marketing de piloter en direct ses indicateurs de performance financiers mondiaux.

---

## 💼 Expérience & Leadership

###  Optimisation et Administration logistique (Bénévolat)
**Secours Populaire Français du Haut-Rhin (France)** | *02/2026 - Aujourd'hui*
* Analyse des flux d'entrées et de sorties de stock.
* Traitement des anomalies de saisie et modélisation de la rotation des stocks.
* Conception d'outils de pilotage décisionnels visuels pour améliorer la distribution et l'allocation des ressources aux bénéficiaires.

### 💻 Technicien informatique & support IT
**COMPUTER FOREVER (Togo)** | *2022 - 2024*
* Maintenance, diagnostic et résolution de problèmes matériels et logiciels pour les PME et PMI.
* Support aux utilisateurs et gestion d'outils numériques avec une approche analytique et rigoureuse.
* Réduction de 25% des incidents système critiques et contribution directe à l'augmentation de 15% du portefeuille client.

---

## 🎓 Formation

* 🎓 **Master 2 Ingénierie Mathématique & Data Science** – Université de Haute-Alsace (UHA) | *2026 - 2027*
* 🎓 **Licence Mathématiques Appliquées** – Université de Haute-Alsace (UHA) | *2024 - 2025*
* 🎓 **Licence Fondamentale de Mathématiques** – Université de Lomé | *2019 - 2023*

---

## 📜 Certifications, Langues & Soft Skills

### 🏅 Certifications Internationales
* ![DeepLearning.AI](https://img.shields.io/badge/Spécialisation_Machine_Learning-DeepLearning.AI_%26_Stanford-2962FF?style=flat-square&logo=analytics)
* ![Google](https://img.shields.io/badge/Google_Data_Analytics_Certificate-Google-4285F4?style=flat-square&logo=google)
* ![Fraud](https://img.shields.io/badge/Certification_IA_in_Fraud_Detection-Active-success?style=flat-square)

### 🗣️ Langues
* ![Français](https://img.shields.io/badge/Français-Natif-brightgreen?style=flat-square)
* ![Anglais](https://img.shields.io/badge/Anglais-B2-blue?style=flat-square)

### 🧠 Soft Skills
* **Autodidacte et curieux** : Capacité à apprendre et à m'adapter rapidement face à de nouvelles architectures de données ou problématiques métiers.
* **Esprit attentif et communicant** : Facilitateur de collaboration et de compréhension mutuelle au sein d'équipes pluridisciplinaires (techniques et décisionnelles).
