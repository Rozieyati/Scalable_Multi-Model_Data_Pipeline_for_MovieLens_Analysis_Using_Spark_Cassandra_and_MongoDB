<div align="center">

# 🎬 Scalable Multi-Model Data Pipeline
## Integrating Apache Spark, Cassandra, and MongoDB for MovieLens Analysis

![Apache Spark](https://img.shields.io/badge/Apache%20Spark-3.x-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Apache Cassandra](https://img.shields.io/badge/Apache%20Cassandra-AstraDB-1287B1?style=for-the-badge&logo=apachecassandra&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)

*A cloud-native polyglot persistence architecture for scalable movie recommendation analytics.*

</div>

---

# 📖 Project Overview

This project presents a **Scalable Multi-Model Data Pipeline** developed using **Apache Spark**, **Apache Cassandra (DataStax Astra DB)**, and **MongoDB Atlas** for analysing the **MovieLens 100K** dataset.

Instead of relying on a traditional relational database, this project adopts a **Polyglot Persistence** architecture where each database technology is selected based on its strengths:

- ⚡ Apache Spark → Distributed ETL & Data Processing
- 📊 Apache Cassandra (Astra DB) → Analytical Storage
- 👤 MongoDB → Operational User Profile Storage

The architecture separates analytical workloads from operational workloads to improve scalability, flexibility, and query performance.

---

# 🏗 System Architecture

```
                    MovieLens Dataset
          (u.data | u.user | u.item)

                     │
                     ▼

           Apache Spark (Distributed ETL)

                     │
          ┌──────────┴──────────┐
          ▼                     ▼

 Apache Cassandra         MongoDB Atlas
 (Analytical Data)      (Operational Data)

          │                     │
          └──────────┬──────────┘
                     ▼

          Exploratory Data Analysis
          Dashboard Visualisation
```

---

# 🚀 Technologies Used

| Technology | Purpose |
|------------|---------|
| Apache Spark | Distributed ETL & Processing |
| Apache Cassandra (Astra DB) | Analytical Data Storage |
| MongoDB Atlas | Operational User Profiles |
| Python | Data Engineering |
| PySpark | Distributed Data Processing |
| Plotly | Interactive Visualisation |
| Matplotlib | Statistical Charts |
| Pandas | Data Manipulation |

---

# 📂 Dataset

**MovieLens 100K**

The dataset contains:

- 🎥 100,000 Movie Ratings
- 👥 943 Users
- 🎬 1,682 Movies

Dataset Source:

https://grouplens.org/datasets/movielens/

---

# 🔄 Data Pipeline

### Phase 1 — Data Acquisition

- Load MovieLens dataset
- Schema validation
- Data cleaning

### Phase 2 — Distributed ETL

- Apache Spark
- Data Integration
- Aggregation
- Feature Engineering

### Phase 3 — Polyglot Persistence

### Apache Cassandra

Stores:

- Movie Rankings
- Average Ratings
- Review Counts

### MongoDB

Stores:

- User Profiles
- Demographic Information
- Geographic Information

### Phase 4 — Exploratory Data Analysis

Visualisation and analytical reporting.

---

# 📊 Visualisations

## Apache Cassandra Analytics

- ⭐ Top Rated Movies
- 🎬 Most Popular Movies
- 📈 Rating Distribution
- 💬 Rating vs Review Count

---

## MongoDB Analytics

- 👥 Age Distribution
- 🚻 Gender Distribution
- 💼 Occupation Distribution
- 🔥 Occupation × Gender Heatmap
- 🌡 Occupation × Age Heatmap
- 🌎 Regional Distribution

---

# 📈 Key Findings

✔ Apache Spark successfully handled distributed ETL.

✔ Apache Cassandra efficiently stored aggregated analytical metrics.

✔ MongoDB provided flexible storage for heterogeneous user profiles.

✔ Polyglot Persistence improved scalability by separating analytical and operational workloads.

✔ The proposed architecture successfully supported multidimensional analytical exploration.

---

# 📁 Project Structure

```
MovieLens-Pipeline/

│
├── data/
│     ├── u.data
│     ├── u.user
│     └── u.item
│
├── notebooks/
│     └── MovieLens_Pipeline.ipynb
│
├── images/
│     ├── architecture.png
│     ├── charts/
│     └── screenshots/
│
├── report/
│     └── Final_Report.pdf
│
├── README.md
│
└── requirements.txt
```

---

# 📌 Research Objectives

- Develop a distributed ETL pipeline using Apache Spark.

- Implement a Polyglot Persistence architecture using Cassandra and MongoDB.

- Perform multidimensional analysis on user interactions.

- Evaluate analytical performance using distributed storage.

- Demonstrate a scalable cloud-native data engineering solution.

---

# 📚 References

- Harper & Konstan (2016)
- Han, Kamber & Pei (2012)
- Brewer (2012)
- Kleppmann (2017)
- Zaharia et al. (2016)

---

# 🎓 Academic Information

**Project Title**

> **Scalable Multi-Model Data Pipeline: Integrating Apache Spark, Cassandra, and MongoDB for MovieLens Analysis**

---

# 📧 Author

**Rozieyati Azizahtul Asyikin Bte Rozaini**

Master of Science (Data Science & Analytics)

Course Project — Data Management

---

<div align="center">

### ⭐ If you found this project useful, consider giving it a star ⭐

</div>
