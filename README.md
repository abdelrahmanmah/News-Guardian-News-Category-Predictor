# 📰 News Guardian | AI News Category Predictor

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-App-ff4b4b)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Enabled-orange)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Powered-yellow)
![Status](https://img.shields.io/badge/Status-Active-success)

**News Guardian** is a powerful Natural Language Processing (NLP) application designed to classify news articles into their respective categories (Business, Technology, Politics, Sports, and Entertainment) using an ensemble of Machine Learning and Deep Learning models.

The project consists of a comprehensive Jupyter Notebook for model development and a modern Streamlit web application for real-time predictions.

---

## 🚀 Features

### 🧠 Advanced AI Models
- **Ensemble Approach**: Utilizes multiple models to ensure high confidence predictions.
  - **Logistic Regression**: Reliable baseline for text classification.
  - **Random Forest**: Captures non-linear complex patterns.
  - **Support Vector Machine (SVM)**: Effective for high-dimensional text data.
  - **LSTM (Deep Learning)**: Recurrent Neural Network for context-aware sequence processing.

### ✨ Modern Web Interface
- **Use-Friendly Design**: Clean, responsive UI built with Streamlit.
- **Real-Time Analysis**: Instant categorization with confidence scores.
- **Interactive Visualizations**: Dynamic probability charts using Plotly.
- **Robust Error Handling**: Gracefully handles missing dependencies (runs even without TensorFlow/LSTM).

---

## 📂 Project Structure

```
├── BBC_news_data/               # Raw dataset
├── News_Category_Prediction.ipynb # Database analysis, EDA, and Model Training
├── app.py                       # Streamlit Application Entry Point
├── requirement.txt              # Project dependencies
└── README.md                    # Project Documentation
```

---

## 🛠️ Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/news-guardian.git
cd news-guardian
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```
*Note: Ensure `tensorflow` is installed for Deep Learning capabilities.*

### 3. Generate Models (Optional)
If model artifacts (`.pkl` or `.h5` files) are missing, generate them using:
```bash
python generate_models.py
```

---

## 🖥️ Usage

### Running the Web App
Launch the Streamlit interface:
```bash
streamlit run app.py
```
The app will open in your default browser (usually at `http://localhost:8501`).

### How to Use
1.  **Paste Text**: Copy a news headline or article body into the text area.
2.  **Analyze**: Click the **"Analyze & Predict Category"** button.
3.  **View Results**:
    - See the predicted category and confidence score for each model.
    - Explore the probability distribution chart to see how confident the models are across all categories.

---

## 📊 Model Performance

The models were trained on the **BBC News Dataset**, achieving high accuracy metrics:

| Model | Accuracy | Strengths |
|-------|----------|-----------|
| **XGBoost** | ~98% | High performance, gradient boosting power. |
| **Random Forest** | ~97% | Robust against overfitting. |
| **Logistic Regression** | ~96% | Fast interpretabiltiy. |
| **LSTM** | *Variable* | Captures sequential context best. |

*Detailed evaluation and EDA can be found in `News_Category_Prediction.ipynb`.*

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).
