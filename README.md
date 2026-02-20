# 🌞 Solar Flare Early Warning using Attention LSTM

An end-to-end deep learning system for **early solar flare risk forecasting** combining RHESSI flare events, temporal activity features, and GOES X-ray flux.

The project explores how sequence models capture precursor activity and evaluates performance using space-weather metrics such as **ROC-AUC, PR-AUC, and TSS**.

---

## 🚀 Overview

Solar flares are rare, high-impact space-weather events that can affect satellites, communication systems, and power grids.

Traditional classification approaches struggle due to extreme class imbalance and temporal buildup before flares.

This project reframes flare prediction as an **early warning time-series problem** using:

- Event sequences  
- Activity memory features  
- Physical X-ray flux (GOES)  
- Attention-based LSTM  

The system outputs **probabilistic risk timelines** instead of simple binary predictions.

---

## 🧠 Methodology

### Data Sources
- RHESSI flare event catalogue  
- GOES X-ray flux time series  

### Feature Engineering
- Time-gap features  
- Rolling activity statistics  
- Lagged GOES precursor signals  
- Long-window sequence construction  

### Modeling Approach
- LSTM baseline  
- Attention LSTM architecture  
- Early-warning labeling formulation  
- Threshold calibration for TSS optimization  

---

## 📊 Results

Performance on rare-event flare forecasting:

- **ROC-AUC:** ~0.69  
- **PR-AUC:** ~0.29  
- **TSS:** ~0.30  

### Key Findings
- Temporal memory improves regime detection  
- Attention sharpens precursor sensitivity  
- GOES fusion smooths risk estimation  
- Event-only datasets impose a performance ceiling  

---

## 🖥️ Streamlit Dashboard

The interactive dashboard provides:

- Risk timeline visualization  
- Predicted alert windows  
- Dataset preview  
- Adjustable decision threshold  
- Model configuration overview  

🔬 Research Insights

This project demonstrates:

Early-warning framing is more effective than point prediction

Physical signals improve calibration more than architecture alone

Rare-event forecasting requires PR-AUC and TSS evaluation

Performance plateaus highlight data limitations rather than model failure

🧭 Future Work

Magnetic field (HMI/SHARP) feature integration

Multi-horizon forecasting (6h / 12h / 24h)

Ensemble calibration methods

Attention interpretability

Real-time streaming inference

👤 Author

Sarthak Jagota

Interests:

Machine Learning for Science

Space Weather Forecasting

Time-Series Modeling

Deep Learning Interpretability
