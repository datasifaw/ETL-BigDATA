# ETL-BigDATA
# 📦 Mini-Projet ETL Big Data – Kafka, PySpark, MongoDB

## 👨‍💻 Réalisé par : AZOUGHLI Said

## 🎯 Objectif
Mettre en place une pipeline ETL temps réel :
- Générer des événements utilisateur avec **Kafka**
- Traiter et enrichir les données avec **PySpark Streaming**
- Sauvegarder les données dans **MongoDB**
- Analyser et visualiser les données avec **Pandas / Matplotlib**

---

## ⚙️ Technologies utilisées

- Apache Kafka 📨
- Apache Spark (PySpark) ⚡
- MongoDB (via Docker) 🗄️
- Python (Kafka Producer + Visualisation)
- Jupyter Notebook

---

## 📁 Structure du projet

```
bigdata-etl-project/
├── docker-compose.yml           # Lancement de Kafka, Zookeeper, MongoDB
├── producer.py                  # Génère 1000 événements Kafka simulés
├── spark_streaming.py           # Lit les événements Kafka en streaming (console)
├── etl_to_mongodb.py            # Traite & insère les données enrichies dans MongoDB
├── check_mongo.py               # Vérifie le contenu MongoDB
├── analysis.ipynb               # Analyse & visualisation des données
├── etl_pipeline_analysis_maroc.ipynb  # Notebook avec analyse spécifique sur le Maroc 🇲🇦
├── *.png                        # Graphiques générés (matplotlib/seaborn)
└── README.md                    # Ce fichier 📄
```

---

## ▶️ Lancement rapide

1. Démarrer les services :
```bash
docker-compose up -d
```

2. Générer les messages Kafka :
```bash
python producer.py
```

3. Lancer le traitement Spark :
```bash
python etl_to_mongodb.py
```

4. Analyser les résultats :
- Lancer `analysis.ipynb` dans Jupyter
- Ou utiliser le notebook Maroc

---

## 🇲🇦 Bonus
Analyse dédiée pour les données `location == "MA"` avec graphe + moyenne des achats.

---

## ✅ Résultat attendu

- Pipeline complet : **Kafka → Spark → MongoDB → Visualisation**
- Graphiques clairs et filtrés
- Notebook prêt à remettre

---
---

## ✅ Conclusion

Ce projet m'a permis, de concevoir et mettre en œuvre un pipeline ETL temps réel complet basé sur Kafka, PySpark et MongoDB.  
j'ai appris à gérer des flux de données, à les transformer en streaming, et à les exploiter via des visualisations claires.
  
L’ajout d’une analyse spécifique au **Maroc** 🇲🇦 a permis de contextualiser les résultats.

Ce projet a été une excellente introduction pratique aux architectures Big Data utilisées en entreprise.
