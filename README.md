# Sarcasm Detection in Dravidian Code-Mixed Social Media Texts (2024)

![Sarcasm Detection Banner](https://img.shields.io/badge/Sarcasm-Detection-green.svg)
![Dravidian Languages](https://img.shields.io/badge/Dravidian-CodeMix-blueviolet.svg)
![License](https://img.shields.io/github/license/muru2005/Sarcasm-Detection-Dravidian-CodeMix-2024)

## 🚀 Introduction

Welcome to the **Sarcasm Detection in Dravidian Code-Mixed Social Media Texts (2024)** repository!  
This project tackles the nuanced challenge of detecting sarcasm in social media posts written in code-mixed Dravidian languages (primarily Tamil, Malayalam, Kannada, and English).  
Our solutions leverage cutting-edge Natural Language Processing (NLP) techniques and deep learning architectures to push the boundaries of sarcasm detection in multilingual, code-mixed scenarios.

## 🎯 Motivation

Social media conversations in South India often feature code-mixing between Dravidian languages and English, making sarcasm detection harder than in monolingual contexts.  
Sarcasm can subtly change the meaning and sentiment of a message, impacting tasks like sentiment analysis, moderation, and user experience.  
**This repository is dedicated to advancing research and practical tools for automatic sarcasm detection in these complex linguistic environments.**

## 🧑‍💻 Core Features

- **Multilingual Support:** Works with Tamil, Malayalam, Kannada, and English code-mixed texts.
- **State-of-the-Art Models:** Implements transformer-based architectures, including mBERT, XLM-R, and custom LSTM/GRU solutions.
- **Flexible Data Pipeline:** Easily ingest, preprocess, and augment code-mixed datasets.
- **Explainability:** Includes interpretable outputs and visualizations to understand model decisions.
- **Ready for Research and Deployment:** Modular code can be adapted for academic research or production systems.

## 📦 Repository Structure

```
Sarcasm-Detection-Dravidian-CodeMix-2024/
├── data/                 # Datasets: raw, preprocessed, splits
├── notebooks/            # Jupyter notebooks for exploration and EDA
├── src/                  # Source code: models, preprocessing, utils
│   ├── models/           # Model architectures and training scripts
│   ├── preprocessing/    # Text normalization, code-mix handling
│   └── utils.py          # Helper functions
├── results/              # Evaluation results, metrics, visualizations
├── requirements.txt      # Python dependencies
├── README.md             # This file
└── LICENSE
```

## 🚦 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/muru2005/Sarcasm-Detection-Dravidian-CodeMix-2024.git
cd Sarcasm-Detection-Dravidian-CodeMix-2024
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download and Prepare Data

- Place your dataset files in the `data/` directory.
- Use the provided preprocessing scripts in `src/preprocessing/` to clean and format your data.

### 4. Train the Model

```bash
python src/train.py --config configs/config.yaml
```

### 5. Evaluate & Visualize

- Results and visualizations will be saved in `results/`.
- Use notebooks in `notebooks/` for further analysis.

## 📊 Example: Dataset Format

```csv
text,label
"Enna sir ippadi panreenga? Amazing!",sarcastic
"Nice job!",not_sarcastic
```

Supports code-mixed texts like:
- "Super ah irukku, what an idea!"
- "Innu ithu work aagum nu ninaichiya?"

## 🧠 Models Implemented

- **mBERT / XLM-R:** Pre-trained multilingual transformer models.
- **Custom LSTM/GRU architectures:** For sequence modeling.
- **Hybrid Approaches:** Combining classical features (TF-IDF, sentiment scores) with deep learning.

## 📈 Results

| Model           | F1-Score | Accuracy |
|-----------------|----------|----------|
| mBERT           | 0.81     | 82%      |
| XLM-R           | 0.83     | 84%      |
| LSTM (baseline) | 0.72     | 74%      |

*(Refer to `results/` for full metrics and analysis)*

## 🧩 Extensibility

- Add new languages or models by extending `src/models/`.
- Plug in external datasets.
- Integrate with web APIs for real-time sarcasm detection.

## 🦸‍♂️ Contributing

We welcome contributions! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.  
Open issues or submit pull requests for features, bug fixes, or improvements.

## 🤝 Acknowledgements

- Inspired by the [LT-EDI Shared Task on Sarcasm Detection in Dravidian Languages](https://github.com/DravidianLangTech/lt-edi-2024).
- Thanks to all dataset creators and annotators.

## 📄 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## ❓ FAQ

- **Which languages are supported?** Tamil, Malayalam, Kannada, and English code-mixed text.
- **Can I use my own dataset?** Yes, follow the format in the `data/` directory.
- **How do I report bugs?** Open an issue in this repository.

---

> *Detecting sarcasm in multilingual contexts is hard. We're making it easier—one byte at a time.*
