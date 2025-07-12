# Bayesian Network Inference GUI

This is an interactive web-based application built with **Streamlit** that allows users to perform probabilistic inference on a **Bayesian Network** model. It supports real-time prediction, feature influence analysis, correlation heatmaps, and 3D visualization of the network structure.

---

## 🔍 Features

- **Bayesian Inference:** Enter known variables to predict unknown ones using the `pgmpy` inference engine.
- **Correlation Heatmap:** Visualizes correlations between numeric features from the original dataset.
- **Feature Influence:** Uses Mutual Information to estimate how much each feature influences the selected target.
- **3D Network Visualization:** Displays a 3D interactive structure of the Bayesian Network using `plotly`.

---

## 🧠 Model & Data Files

✅ **Pre-trained Model File Included:**  
The file `model.pkl` is a trained Bayesian Network model saved using `joblib`. This model is automatically loaded by the application.

✅ **Dataset Required:**  
The application expects `your_dataset.csv` (used during training) to be present in the same folder to enable visualizations and feature analysis.

---

## 🛠️ Tech Stack

- **Python**
- **Streamlit** (GUI)
- **pgmpy** (Bayesian inference)
- **Pandas, NumPy** (Data processing)
- **Seaborn, Matplotlib** (Visualization)
- **Plotly** (3D network graphs)
- **scikit-learn** (Mutual information for feature importance)
- **NetworkX** (Graph structure)

---

## 🗂️ File Structure

```

├── app.py                  # Main Streamlit app
├── model.pkl               # ✅ Trained Bayesian Network model (included)
├── your\_dataset.csv        # Dataset required for heatmap & influence analysis
├── README.md               # Project documentation

````

---

## 🚀 How to Run the App

1. Clone the repository or download the files.
2. Make sure both `model.pkl` and `your_dataset.csv` are in the root directory.
3. Install dependencies:

```bash
pip install -r requirements.txt
````

4. Run the app:

```bash
streamlit run app.py
```

5. In the sidebar, enter evidence values and select a target variable for inference.

---

## 📌 Notes

* Ensure the dataset column names exactly match the Bayesian Network node names.
* Non-numeric fields are auto-encoded before calculating feature influence.
* The model uses **MAP (Maximum A Posteriori)** inference via `pgmpy`.

---

## 📷 Sample Outputs

* ✅ Predicted value of the selected target
* ✅ Feature influence bar chart
* ✅ Correlation heatmap
* ✅ 3D graph of the Bayesian Network

---

## ✍️ Author

**Gurupriya Kannan**
AI/ML Developer | Data Analyst | Frontend Developer
[LinkedIn](https://www.linkedin.com/) | [GitHub](https://github.com/) | [Portfolio](#)

---

## 📜 License

This project is for academic and demonstration purposes. Attribution required if reused.

