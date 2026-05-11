# 👥 Analyse RFM – Segmentation Clients

Projet complet de segmentation client par la méthode RFM (Récence, Fréquence, Montant), incluant l'analyse Python, le dataset, un dashboard Power BI interactif et ses captures d'écran.

---

## 📁 Structure du projet

```

/
├── Données/
│   └── dataset_ventes.csv
├── Python/
│   └── Analyse client sur RFM.ipynb
├── Tableau de bord/
│   └── Dashboard.pbix
└── Captures du tableau de bord/
├── Tableau de bord accueil.png
├── Tableau de bord Matrice RFM.png
├── Segment du tableau de bord.png
└── Tableaux de bord marketing.png

```

---

## 🎯 Objectif

Appliquer la méthode RFM pour segmenter les clients selon leur comportement d'achat et créer un dashboard interactif permettant d'explorer les différents segments et d'identifier les clients à fort potentiel.

---

## 📖 Qu'est-ce que l'analyse RFM ?

La méthode RFM est une technique de segmentation comportementale qui évalue chaque client sur trois critères :

| Critère | Définition | Signification |
|---------|-----------|---------------|
| **Récence (R)** | Date du dernier achat | Plus c'est récent, plus le client est engagé |
| **Fréquence (F)** | Nombre d'achats sur une période | Plus c'est fréquent, plus le client est fidèle |
| **Montant (M)** | Dépense totale cumulée | Plus c'est élevé, plus le client est rentable |

Chaque client reçoit un score de **1 à 5** sur chaque axe (1 = faible, 5 = excellent), ce qui permet de créer des segments exploitables.

---

## 📊 Les segments clients identifiés

| Segment | Score RFM | Description | Action recommandée |
|---------|-----------|-------------|-------------------|
| 🏆 **Champions** | 5-5-5 | Meilleurs clients, fidèles et rentables | Programme de fidélité premium |
| 💎 **Clients fidèles** | 4-5/5-4-4 | Clients réguliers à bon potentiel | Ventes croisées, up-sell |
| ⚠️ **Clients à risque** | 3-3-3 | Anciens bons clients en perte de vitesse | Campagne de réactivation |
| 😴 **Clients perdus** | 1-1-1 | N'ont plus acheté depuis longtemps | Campagne de reconquête ou abandon |
| 🆕 **Nouveaux clients** | 5-1-1 | Achat récent mais unique | Campagne de bienvenue, 2ème achat |

---

## 🔍 Étapes de l'analyse

1. **Importation et nettoyage des données** 
   - Traitement des dates, valeurs manquantes, doublons
   - Vérification des types de données

2. **Analyse exploratoire (EDA)**
   - Distribution des ventes dans le temps
   - Top clients par chiffre d'affaires
   - Saisonnalité des achats

3. **Calcul des scores RFM**
   - Définition de la date de référence
   - Calcul de la récence (jours depuis le dernier achat)
   - Calcul de la fréquence (nombre de transactions)
   - Calcul du montant (somme des dépenses)
   - Attribution des scores de 1 à 5 par la méthode des quintiles

4. **Segmentation des clients**
   - Création des groupes selon la combinaison des scores
   - Analyse de la répartition des segments
   - Profilage de chaque segment

5. **Visualisations et dashboard**
   - Matrice RFM interactive
   - Répartition des segments
   - Détail par client
   - Recommandations marketing par segment

---

## 🛠 Outils utilisés

| Catégorie | Outils |
|-----------|--------|
| Langage | Python 3 |
| Notebook | Jupyter Notebook |
| Librairies | Pandas, NumPy, Matplotlib, Seaborn |
| Dashboard | Microsoft Power BI |

---

## 📸 Aperçu du Dashboard RFM

### Voir dossier "Dashboard_capture"

---

## 🚀 Comment utiliser ce projet

### Prérequis
- Python 3.x installé
- Power BI Desktop (gratuit) pour le dashboard
- Git pour cloner le dépôt

### Installation et exécution

1. **Cloner le dépôt**
   bash
   git clone https://github.com/NourLuz/analyse-ventes-clients.git
   cd analyse-ventes-clients/Projet-RFM
