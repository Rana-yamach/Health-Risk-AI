# 🇹🇷 AI Health Policy Simulator (Turkey)

An interactive Machine Learning application that simulates how dietary habits and demographic factors impact cardiovascular mortality rates. Designed for policymakers and health officials, this tool uses a **Random Forest** model to predict health outcomes and generate actionable policy interventions.

## 🚀 Live Demo
*(https://huggingface.co/spaces/sakurana/health-policy-simulator-turkey)*

---

## 🎯 Project Overview
Cardiovascular disease is a leading cause of global mortality. This project aims to move beyond static statistics by providing a dynamic **"What-If" simulator**. Users can adjust macro-level variables (e.g., national wheat consumption, sugar intake, demographic shifts) to see instant predictions on mortality risk.

**Key Question:** *How would a 20% reduction in sugar consumption or a subsidy on vegetables impact heart disease mortality in Turkey?*

---

## ✨ Features
* **Predictive Engine:** Uses a trained Random Forest Regressor (R² ~0.85) to forecast cardiovascular mortality rates.
* **Interactive Simulation:** Streamlit-based UI allows real-time adjustment of policy levers (Wheat, Sugar, Veggies, etc.).
* **Smart Policy Insights:** Automatically generates context-aware government recommendations (e.g., "Implement SSB Tax", "Subsidize Alternative Grains") based on current slider inputs.
* **Risk Badging:** Visual indicators for "High Risk" vs "Optimal" dietary zones.

---

## 🛠️ Tech Stack
* **Frontend:** [Streamlit](https://streamlit.io/)
* **Machine Learning:** Scikit-learn (Random Forest)
* **Data Processing:** Pandas, NumPy
* **Deployment:** Docker / Hugging Face Spaces

---

## 📂 Repository Structure
```text
├── data/                  # Original and processed datasets
├── docs/
├── notebooks/             # Jupyter notebooks for EDA, training, and evaluation
├── src/                   # Source code for the application
│   ├── config.py          # Configuration paths and variables
│   ├── inference.py       # Model loading and prediction logic
│   ├── streamlit_app.py   # Main dashboard application
│   ├── final_model.pkl    # Trained Random Forest model (LFS tracked)
│   └── feature_names.pkl  # List of features used during training
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
