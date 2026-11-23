# Freezing vs Fine-Tuning CNNs

Comparing CNN transfer learning training strategies (Feature Extraction / Layer Freezing vs. Full & Gradual Fine-Tuning) using the **Oxford-IIIT Pet Dataset**.

---

## 📁 Repository Structure

```text
freezing-vs-finetuning-cnn/
├── data/          # Dataset storage (excluded from git tracking)
├── notebooks/     # Exploratory data analysis (EDA) and experimental notebooks
├── src/           # Main source code (models, data loaders, training pipelines)
├── models/        # Model checkpoints and saved weights (excluded from git)
├── results/       # Evaluation metrics, CSV experiment summaries, logs
├── figures/       # Generated charts, loss/accuracy curves, visualizations
├── paper/         # Research paper, reports, and reference literature
├── requirements.txt
└── README.md
```

---

## 🎯 Objectives
- **Feature Extraction (Freezing)**: Freeze pre-trained convolutional backbone weights and train only the classification head.
- **Fine-Tuning**: Unfreeze intermediate/top layers or the entire network with lower learning rates to adapt features to domain-specific patterns.
- **Empirical Comparison**: Quantify differences in convergence speed, final accuracy, computational overhead, and overfitting risks.

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/freezing-vs-finetuning-cnn.git
cd freezing-vs-finetuning-cnn
```

### 2. Environment Setup
Create a virtual environment and install dependencies:
```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# Linux / macOS:
source .venv/bin/activate

pip install -r requirements.txt
```

---

## 📊 Dataset
This study utilizes the [Oxford-IIIT Pet Dataset](https://www.robots.ox.ac.uk/~vgg/data/pets/):
- 37 categories of pets (breeds of cats and dogs)
- Approximately 200 images per class

---

## 📜 License
This project is licensed under the terms described in the [LICENSE](LICENSE) file.
