# 🧠 ANN-Based Customer Churn Predictor

[![Streamlit App](https://img.shields.io/badge/Live%20Demo-Open%20App-brightgreen?logo=streamlit)](https://ann-churn-predictor.streamlit.app/)

A responsive and easy-to-use **Streamlit web application** that predicts the likelihood of a customer leaving a bank using an **Artificial Neural Network (ANN)** built with **TensorFlow**. This project demonstrates how machine learning models can be deployed for real-world decision-making in customer retention strategies.

---

## 🕸️ Model Architecture

The **Artificial Neural Network (ANN)** used for churn prediction consists of:

- **Input Layer**: Receives 11 features after encoding and scaling.
- **Hidden Layer 1**: Dense layer with ReLU activation.
- **Hidden Layer 2**: Dense layer with ReLU activation.
- **Output Layer**: Dense layer with a sigmoid activation to output churn probability between 0 and 1.

> 🔧 The model was trained using the **binary cross-entropy** loss function and the **Adam optimizer**.

---

## 🔍 What is Customer Churn?

**Customer churn** refers to the percentage of customers who stop using a company’s service during a certain time frame. By predicting churn, businesses can take proactive steps to retain high-risk customers and improve satisfaction.

---

## 🚀 Live Demo

👉 **[Click here to try the app](https://ann-churn-predictor.streamlit.app/)**

Enter customer details like credit score, age, geography, balance, and more — and receive an instant prediction on whether the customer is likely to churn.

---

## 🎯 Features

- 🔮 Predicts **churn probability** using a trained ANN model
- 🎛 Handles preprocessing:
  - `LabelEncoder` for gender
  - `OneHotEncoder` for geography
  - `StandardScaler` for feature scaling
- 📊 Displays result in human-readable format with percentage score
- ⚡ Instant prediction inside a clean and interactive **Streamlit interface**

---

## 🧠 Model & Tech Stack

- **Model**: Artificial Neural Network (Keras / TensorFlow)
- **Frontend**: Streamlit
- **Preprocessing**: scikit-learn
- **Data Handling**: pandas, numpy

---

## 📁 Repository Structure

```bash
├── app.py                    # Main Streamlit application
├── model.h5                  # Trained ANN model
├── scaler.pkl                # StandardScaler for numerical features
├── label_encoder_gender.pkl  # LabelEncoder for gender
├── onehot_encoder_geo.pkl    # OneHotEncoder for geography
├── requirements.txt          # Python dependencies
└── runtime.txt               # Python version pinning (e.g., python-3.10)'
```
## 🛠 Setup Instructions (Local)

### 1. Clone the Repository
```bash
git clone https://github.com/ganeshgupta3/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Create Virtual Environment *(Recommended)*
```bash
# Using venv
python -m venv churn_env
source churn_env/bin/activate  # On Windows: churn_env\Scripts\activate

# Using conda
conda create -n churn_env python=3.11
conda activate churn_env
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the App
```bash
streamlit run app.py
```

The app will automatically open in your browser at `http://localhost:8501`

---

## 📦 Dependencies

```txt
tensorflow>=2.16.0
streamlit
pandas
numpy
scikit-learn
tensorboard
matplotlib
```

⚠️ **Note**: This project uses **Python 3.11** to ensure TensorFlow compatibility. The version is specified in `runtime.txt` for Streamlit Cloud deployment.


---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push upstream feature/AmazingFeature`)
5. Open a Pull Request

---

## 📬 Contact

**Ganesh Gupta**
- GitHub: [@ganeshgupta3](https://github.com/ganeshgupta3)
- Project Link: [Customer Churn Predictor](https://github.com/ganeshgupta3/customer-churn-prediction)

---

<div align="center">

**⭐ Star this repo if you found it helpful!**

*Made with ❤️ using Streamlit and TensorFlow*

</div>