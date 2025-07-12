# K-Means Clustering on 20 Newsgroups Dataset

This project applies K-Means clustering to group similar documents from the classic **20 Newsgroups** dataset for topic modeling and understanding large text corpora.

---

## 📚 Project Overview

- **Dataset:** 20 Newsgroups (~20,000 Usenet posts across 20 topics)
- **Goal:** Cluster similar documents into groups corresponding to topics
- **Approach:** 
  - Text preprocessing
  - TF-IDF vectorization
  - K-Means clustering
  - Analysis of top terms per cluster
  - Cluster evaluation

---

## 🔧 How to Run

### 1. Clone the repo (if applicable)

```bash
git clone https://github.com/A-TomMarvoloRiddle/Document-Clustering-with-K-Means-Algo.git
cd <repo-folder>
````

### 2. Install dependencies

Make sure you have Python ≥ 3.7 installed.

Install required libraries:

```bash
pip install scikit-learn numpy pandas
```

### 3. Run the script

```bash
python Project.py
```

---

## ✅ What the Script Does

* Loads the 20 Newsgroups dataset (removing headers/footers/quotes)
* Converts text into TF-IDF vectors
* Runs K-Means clustering (k = 20)
* Prints:

  * Cluster sizes
  * Top terms per cluster (helps identify topics)
  * Sample documents and their cluster assignments
  * Normalized Mutual Information (NMI) score to evaluate clustering quality
* Exports a CSV file containing:

  * document snippet
  * assigned cluster
  * true newsgroup label

---

## 📁 Output Files

* `newsgroups_results.csv`

This CSV file contains:

| document\_snippet | cluster | true\_newsgroup |
| ----------------- | ------- | --------------- |
| ...               | ...     | ...             |

---

## 📝 Example Output

```
Loaded 18846 documents.
TF-IDF matrix shape: (18846, 10000)

Running K-Means with 20 clusters...
Clustering complete.

Top terms per cluster:
Cluster 0: drive, disk, scsi, hard, drives, mac, controller, apple, ide, floppy
Cluster 1: game, team, season, games, players, hockey, year, play, baseball, hit
...

Cluster sizes:
0     641
1     992
2    1207
...

Normalized Mutual Information (NMI): 0.4643
```

---

## 📚 References
* [20 Newsgroups Dataset](http://archive.ics.uci.edu/ml/datasets/Twenty+Newsgroups)

---
