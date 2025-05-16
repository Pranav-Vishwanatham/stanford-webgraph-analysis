
# 📊 Stanford Web Graph Analysis

This project explores a subgraph of Stanford’s 2002 Web Graph dataset to study complex network structures and behaviors. Using tools such as NetworkX, PyTorch, Gephi, and Pyvis, we analyze connectivity, rank nodes, predict future links, and detect community clusters within the web graph.

## 📌 Summary

The original dataset contains 281,903 nodes and over 2.3 million edges. Due to computational constraints, we sampled it down to 13,142 nodes and 359,114 edges. The analysis focuses on:

- 🔗 **Link Prediction** using:
  - Adamic-Adar Index
  - Preferential Attachment
  - Graph Convolutional Networks (GCNs)
- ⭐ **PageRank Evaluation** using:
  - Classic PageRank
  - Heat Kernel PageRank
- 🧠 **Community Detection** using modularity and dendrogram analysis
- 📈 **Network Metrics** such as average degree, path length, modularity, and clustering coefficient
- 🌐 **Interactive Graph Visualization** using Pyvis and Gephi

All methods and results are explained in the project report:  
📄 [Report.pdf](./Report.pdf)

---

## 📁 Project Structure

```
├── Dataset/
│   └── subgraph.csv, web-Stanford.txt.gz
├── Gephi/
│   └── Web graph Project.gephi
├── Source code/
│   ├── CommunityDetection.ipynb
│   ├── LinkPrediction_SMA.ipynb
│   ├── Page_Rank_Analysis.ipynb
│   └── Visualization.ipynb
├── Report.pdf
└── README.md
```

---

## 📊 Key Results

| Metric                     | Value     |
|---------------------------|-----------|
| Average Degree            | 27.33     |
| Graph Density             | 0.002     |
| Modularity                | 0.796     |
| Clustering Coefficient    | 0.507     |
| Avg Path Length           | 8.514     |

- PageRank MAE ≈ 0.000093  
- PageRank RMSE ≈ 0.000492  

GCN link prediction achieved **AUC-ROC score of 0.9995** at best learning rate.

---

## 🔧 Requirements

Some of the key libraries used:

- `networkx`
- `pyvis`
- `pandas`
- `matplotlib`
- `torch`
- `numpy`
- `gephi` (desktop tool)


---


## 📂 Dataset Source

Stanford Web Graph Dataset (2002):  
🔗 [https://snap.stanford.edu/data/web-Stanford.html](https://snap.stanford.edu/data/web-Stanford.html)

---

