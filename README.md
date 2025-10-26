# GraphDTA Reproduction

This repository reproduces the experiments from the paper:

**GraphDTA: Predicting drug–target binding affinity with graph neural networks**  
*Thin Nguyen et al., Bioinformatics, 2021*

---

## 🧠 Overview

GraphDTA is a deep learning model that predicts the **binding affinity** between drugs and target proteins.  
It represents **drugs as molecular graphs** and uses **graph neural networks (GCN, GAT, GIN)** combined with CNNs on protein sequences.

This reproduction aims to replicate the reported results on the **Davis** and **KIBA** datasets using **PyTorch Geometric** and **RDKit**.

---

## ⚙️ Installation

```bash
git clone https://github.com/ghyiasmir/GraphDTA-Reproduction.git
cd GraphDTA-Reproduction
pip install -r requirements.txt
```

---

## 📁 Folder Structure

```
GraphDTA-Reproduction/
│
├── src/                   # Source code for models, training, evaluation
├── notebooks/             # Jupyter notebook for demonstration
├── results/               # Store outputs, logs, checkpoints
├── requirements.txt       # Python dependencies
└── README.md              # Project overview
```

---

## 🚀 How to Run

**Option 1: Run in Google Colab**
1. Open `notebooks/GraphDTA_Reproduction.ipynb` in Colab.  
2. Follow the cells step-by-step.

**Option 2: Run Locally**
```bash
python src/train.py --model GCN --dataset KIBA
```

---

## 📊 Evaluation Metrics
- **Mean Squared Error (MSE)** — lower is better  
- **Concordance Index (CI)** — higher is better

---

## 🧩 Model Variants
- `GCN` — Graph Convolutional Network  
- `GAT` — Graph Attention Network  
- `GIN` — Graph Isomorphism Network  
- `GAT-GCN` — Hybrid model

---

## 👨‍💻 Author
**Ghyias Mir**  
Software Engineer | AI Researcher  
📧 Email: mirghyias@gmail.com  
🔗 GitHub: [ghyiasmir](https://github.com/ghyiasmir)

---

## 📚 Reference
Nguyen, T., Le, H., Quinn, T. P., Nguyen, T., Le, T. D., & Venkatesh, S. (2021).  
*GraphDTA: Predicting drug–target binding affinity with graph neural networks.*  
Bioinformatics, 37(8), 1140–1147. [DOI:10.1093/bioinformatics/btaa921]

