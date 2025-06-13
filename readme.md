# Bot Cluster ATAS

Backtest et développement d’un bot de trading basé sur les clusters significatifs de Bid & Ask dans ATAS.

---

## 🧠 Contexte

Lors de mes analyses manuelles, j'ai observé que certains clusters sous forme de gros ordres limits provoquent régulièrement une réaction significative du prix.

J’ai donc effectué un premier backtest manuel, en mesurant l’ATR 5 minutes maximal atteint dans le sens et à l’encontre de chaque cluster.

Y'a clairement quelque chose à faire, mais j'ai besoin de beaucoup plus de données et je ne peux pas faire ça à la main.

Donc je fais d'une pierre deux coups ; Un bot de backtest pour trouver le sweet spot de chaque actif testé. Et ce code servira de base pour construire un bot de trading basé sur les clusters.

---

## 🎯 Objectifs du projet

1. Automatiser le backtest sur plusieurs actifs :

   - Détection des clusters
   - Calcul des mouvements de prix post-cluster
   - Évaluation des TP/SL exprimés en multiples d’ATR

2. Concevoir un bot de trading autonome :

   - Capable d'exploiter ces clusters en temps réel
   - Connecté à l'exchange Bitget via leur API
   - Piloté par les résultats du backtest

---

## 🔧 Stack technique

- Logiciel d’analyse : ATAS
- Langage : Python 3.12.7
- Backtest & traitement : Pandas, NumPy, etc.
- Bot trading (à venir) : API Bitget

📂 Organisation du projet


Bot-Cluster-ATAS/
│
├── data/ # Données extraites ou générées
├── notebooks/ # Prototypes et explorations
├── src/ # Code source principal
├── README.md # Ce fichier
└── requirements.txt # Dépendances du projet (à venir)



---

## 🚧 Avancement

- [x] Structuration du projet
- [ ] Scripts d’import et de détection des clusters
- [ ] Script de backtest multi-actif
- [ ] Analyse des taux de réussite TP/SL
- [ ] Développement du bot live
