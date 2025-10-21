# 🧠 Multi-Agent MBTI-Inspired Cognitive AI for Enhanced Cybersecurity Threat Detection and Analysis

### Author: [Suhani Verma](https://github.com/suhaniverma)
**Affiliation:** Banasthali Vidyapith  
**Keywords:** MBTI · Multi-Agent Systems · Cybersecurity · Cognitive AI · Intrusion Detection · Cognitive Diversity  

---

## 📘 Overview

This repository contains the implementation and research work of **"Multi-Agent MBTI-Inspired Cognitive AI for Enhanced Cybersecurity Threat Detection and Analysis"**, a novel Intrusion Detection System (IDS) framework that applies **human-inspired cognitive diversity** using the **Myers-Briggs Type Indicator (MBTI)** model.

The framework models **16 autonomous agents**, each simulating a distinct MBTI cognitive profile through **RandomForest-based AI agents**. This approach introduces **cognitive diversity** into machine learning for cybersecurity — improving generalization, robustness, and adaptability against evolving threats.

---

## 🧩 Abstract

> We propose a Multi-Agent MBTI-Inspired Cognitive AI framework that enhances IDS performance by mimicking human cognitive diversity. Each agent is a customized RandomForestClassifier configured based on MBTI cognitive traits.  
> Evaluated on the UNSW-NB15 dataset, the system achieves **90.0% accuracy** and **0.902 F1-score**, outperforming standard Random Forests (74.9%) and competing with neural IDS models (90.3–91.8%).

---

## ⚙️ Architecture

The system consists of four main Python modules:

| File | Description |
|------|--------------|
| `agent_creator.py` | Defines MBTI-based RandomForest configurations and initializes models. |
| `cyber_trainer.py` | Loads and preprocesses the UNSW-NB15 dataset, trains and validates agents. |
| `evaluator.py` | Computes accuracy, precision, recall, F1-score, and visual comparisons. |
| `main.py` | Orchestrates the complete training, testing, and evaluation workflow. |

Each MBTI agent (e.g., ENTP, ISTJ) has unique hyperparameters reflecting its **cognitive traits**.  
For instance:
```python
MBTI_CONFIGS = {
    "ENTP": {"n_estimators": 120, "max_depth": None},
    "ENTJ": {"n_estimators": 100, "max_depth": 10},
    "ISTJ": {"n_estimators": 50, "max_depth": 5, "conservative": True},
}
````

---

## 🧠 Cognitive AI Concept

| MBTI Trait         | AI Behavior Analogy                        |
| ------------------ | ------------------------------------------ |
| **Intuitive (N)**  | Detects abstract, temporal threat patterns |
| **Sensing (S)**    | Focuses on raw, low-level packet data      |
| **Thinking (T)**   | Logical precision and rule-based detection |
| **Feeling (F)**    | Adaptive, context-aware responses          |
| **Judging (J)**    | Conservative, rule-stable configurations   |
| **Perceiving (P)** | Flexible, exploratory learning             |

This **MBTI-inspired architecture** introduces cognitive diversity similar to human analyst teams, leading to enhanced detection of novel cyberattacks.

---

## 📊 Results

| Model                    | Accuracy  | Precision | Recall    | F1-Score  |
| ------------------------ | --------- | --------- | --------- | --------- |
| Random Forest (Baseline) | 74.9%     | 0.75      | 0.75      | 0.75      |
| CNN (Reference)          | 90.3%     | 0.89      | 0.89      | 0.89      |
| LSTM (Reference)         | 91.8%     | 0.92      | 0.92      | 0.92      |
| **ENTP (Ours)**          | **90.0%** | **0.914** | **0.900** | **0.902** |

**Top Performing MBTI Types:**
`ENTP`, `ENTJ`, `INTJ`, and `ENFP` — Intuitive types outperform Sensing ones in detecting novel or subtle threats.

---

## 🧪 Dataset

**Dataset:** [UNSW-NB15](https://research.unsw.edu.au/projects/unsw-nb15-dataset)

* 49 features, 10 attack categories
* 80% training, 20% testing split
* Preprocessed with mean imputation, label encoding, and feature scaling

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/MBTI-Cognitive-AI-IDS.git
cd MBTI-Cognitive-AI-IDS

# Install dependencies
pip install -r requirements.txt

# Train all MBTI agents
python main.py
```

Trained models are saved automatically in the `cyber_ai/` directory as `.pkl` files.

---

## 🧩 Future Work

* 🧬 **MBTI-Specific Features** – Assign time-series inputs to intuitive agents and packet-level to sensing agents.
* ⚖️ **Ensemble Fusion** – Meta-classifier or weighted averaging to combine agent outputs.
* 🧠 **Hybrid Models** – Integrate LSTM (N-types) and CNN (S-types) architectures.
* 🔐 **Federated Learning** – Distributed agents for privacy-preserving IDS.
* 🛰️ **Real-Time SIEM Integration** – For operational cybersecurity systems.

---

## ⚖️ Ethical Considerations

MBTI is used *only as a heuristic for AI diversity simulation*, not for human profiling.
The system ensures data anonymity and bias mitigation in compliance with ethical AI standards.

---

## 🧾 Citation

If you use this repository or build upon this research, please cite:

```
@article{verma2025mbti,
  title={Multi-Agent MBTI-Inspired Cognitive AI for Enhanced Cybersecurity Threat Detection and Analysis},
  author={Verma, Suhani},
  year={2025},
  affiliation={Banasthali Vidyapith}
}
```

---

## 🌐 Author

**Suhani Verma**
AI & Cybersecurity Researcher | ECE Undergraduate (2023–2027)
Passionate about Neuromorphic AI, BCI Systems, and Defense Technologies
📍 Haridwar, India | 🌏 Aspiring to research in Wellington, NZ
📧 Contact: [LinkedIn](https://www.linkedin.com/in/suhani-verma-suv/) · [GitHub](https://github.com/Victory-7)

---

⭐ *If you find this project interesting, don’t forget to star the repo!*

---

