# AIDPSI — AI Developer Productivity & Stress Index

> *Understanding the balance between AI assistance and human cognitive load.*

A machine learning project that analyzes how developers interact with AI tools and predicts their **Stress Level** and **Productivity Score** based on behavioral and performance metrics. Includes a full EDA notebook and an interactive **Streamlit GUI**.

---

## Key Insight

| AI Usage Level | Effect |
|----------------|--------|
| 🟢 Moderate | Boosts productivity significantly |
| 🔴 Excessive | Increases cognitive load → raises stress |

The sweet spot: using AI as a *collaborator*, not a crutch.

---

## ✨ Features

- 📊 **Exploratory Data Analysis** — Visualize productivity–stress trends across developer profiles
- 🤖 **Dual ML Models** — Separate models for stress prediction (Logistic Regression) and productivity prediction (Decision Tree)
- 🖥️ **Interactive GUI** — Streamlit app to enter your own metrics and get live predictions
- 📁 **Pre-trained Models** — `.pkl` files included; no retraining needed to run the app

---

## 📂 Project Structure

```
Productivity-stress-prediction-model/
│
├── data/
│   └── AI_Developer_Performance.csv  # Dataset (13 features, real developer metrics)
│
├── notebooks/
│   └── Analysis.ipynb                # Full EDA, feature engineering & model training
│
├── models/
│   ├── stress_model.pkl              # Trained Logistic Regression (stress prediction)
│   ├── dt_model.pkl                  # Trained Decision Tree (productivity prediction)
│   ├── scaler.pkl                    # StandardScaler for stress model inputs
│   ├── scaler_prod.pkl               # StandardScaler for productivity model inputs
│   ├── features.pkl                  # Feature list for stress model
│   └── features_prod.pkl             # Feature list for productivity model
│
├── GUI.py                            # Streamlit app for live predictions
├── requirements.txt                  # All dependencies
└── README.md
```

---

## Dataset Features

The dataset (`AI_Developer_Performance.csv`) contains the following columns:

| Feature | Description |
|---------|-------------|
| `Hours_Coding` | Daily hours spent writing code |
| `Lines_of_Code` | Lines of code produced per day |
| `Bugs_Found` | Number of bugs identified |
| `Bugs_Fixed` | Number of bugs resolved |
| `AI_Usage_Hours` | Hours spent using AI tools |
| `Sleep_Hours` | Developer's sleep duration |
| `Cognitive_Load` | Self-reported cognitive load score |
| `Task_Success_Rate` | Percentage of tasks completed successfully |
| `Coffee_Intake` | Cups of coffee consumed |
| `Stress_Level` | ⭐ Target — stress score (0–100) |
| `Task_Duration_Hours` | Average time per task |
| `Commits` | Number of code commits |
| `Errors` | Errors encountered during development |

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/RadhikaKapoor383/Productivity-stress-prediction-model.git
cd Productivity-stress-prediction-model
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Explore the Analysis Notebook

```bash
jupyter notebook
```
Open `notebooks/Analysis.ipynb` to walk through the full EDA, model training, and evaluation pipeline.

### 4. Run the Streamlit GUI

```bash
streamlit run GUI.py
```
Enter your developer metrics in the browser interface and instantly see predicted stress and productivity levels.

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.x | Core language |
| Pandas & NumPy | Data manipulation |
| Scikit-learn | ML models & preprocessing |
| Matplotlib & Seaborn | Data visualization |
| Streamlit | Interactive GUI |
| Jupyter Notebook | Analysis & experimentation |
| Joblib | Model serialization (`.pkl`) |

---

## Goal

Help developers and engineering teams understand how AI tool usage affects **cognitive load and burnout risk**, so they can adopt AI assistance more mindfully — staying productive without sacrificing wellbeing.

---

## Contributing

1. **Fork** the repository
2. **Create** a branch: `git checkout -b feature/your-idea`
3. **Commit** your changes: `git commit -m "Add: description"`
4. **Push**: `git push origin feature/your-idea`
5. **Open** a Pull Request

---

## License

Open-source — free for personal, academic, and research use.

---

<p align="center">Built to help developers work smarter, not harder </p>