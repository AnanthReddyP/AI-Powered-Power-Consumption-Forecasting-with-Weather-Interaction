# AI-Powered Power Consumption Forecasting with Weather Interaction

This project presents a comprehensive AI-based solution to forecast power consumption using historical weather and energy usage data. By leveraging deep learning models and explainable AI tools, it provides accurate, interpretable insights to support smart grid operations and energy optimization.

---

## 🎯 Objective

To compare and evaluate the performance of deep learning models (GRU, LSTM, CNN-LSTM, Transformer) and machine learning models (XGBoost) in predicting power consumption based on real-time weather data. Feature explainability is achieved using LIME and SHAP.

---

## 📁 Folder Structure

```
power-consumption-ai-prediction/
├── src/                    # All notebooks
│   ├── data_preprocessing.ipynb
│   ├── exp1_xgb.ipynb → exp3_xgb_optimized.ipynb
│   ├── exp4_lstm.ipynb → exp6_lstm.ipynb
│   ├── exp7_cnnlstm.ipynb → exp10_cnnlstm.ipynb
│   ├── exp11_lstm_trans.ipynb → exp12_lstm_trans.ipynb
│   ├── exp13_gru.ipynb → exp14_gru.ipynb
│   └── exp_results.ipynb
├── explanations/           # LIME HTML outputs
├── docs/                   # Paper + Presentation
│   ├── Final_Paper.pdf
│   └── Final_Presentation.pdf
├── .gitignore
├── LICENSE.txt
└── README.md
```

---

## 🚀 How to Run

1. Install dependencies:
```bash
pip install numpy pandas matplotlib seaborn tensorflow xgboost shap lime
```

2. Run notebooks in this order:
   - `data_preprocessing.ipynb`
   - XGBoost models: `exp1_xgb` → `exp3_xgb_optimized.ipynb`
   - LSTM models: `exp4_lstm` → `exp6_lstm.ipynb`
   - CNN-LSTM: `exp7_cnnlstm` → `exp10_cnnlstm.ipynb`
   - Transformer: `exp11_lstm_trans.ipynb` → `exp12_lstm_trans.ipynb`
   - GRU: `exp13_gru.ipynb` → `exp14_gru.ipynb`
   - View `exp_results.ipynb` for full comparison
   - Open LIME results in `/explanations` folder for model interpretation

---

## 🧠 Models Evaluated

- ✅ **GRU** – Best overall performance: R² = 0.6985, MAE = 0.0115
- ✅ **XGBoost** – Best short-term predictor: R² = 0.9973
- ✅ **CNN-LSTM** – Good for temporal dependencies
- ✅ **Transformer** – Tested on sequential dependencies
- ✅ **LSTM** – Standard time-series baseline

---

## 📊 Key Takeaways

- GRU achieved highest overall performance
- XGBoost excelled in fine-tuned short-term predictions
- LIME and SHAP revealed temperature and humidity as top features

---

## 🧰 Tools & Libraries

- Python, Pandas, NumPy
- TensorFlow/Keras, XGBoost
- SHAP, LIME, Matplotlib, Seaborn

---

## 📜 License

This project is licensed under the MIT License.
