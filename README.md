# 🔄 ANN-Classification-Churn 🔄

[![GitHub stars](https://img.shields.io/github/stars/yourusername/ANN-Classification-Churn?style=social)](https://github.com/yourusername/ANN-Classification-Churn/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/yourusername/ANN-Classification-Churn?style=social)](https://github.com/yourusername/ANN-Classification-Churn/network/members)
[![GitHub issues](https://img.shields.io/github/issues/yourusername/ANN-Classification-Churn)](https://github.com/yourusername/ANN-Classification-Churn/issues)
[![GitHub license](https://img.shields.io/github/license/yourusername/ANN-Classification-Churn)](https://github.com/yourusername/ANN-Classification-Churn/blob/master/LICENSE)

## 📋 Overview

This repository contains a customer churn prediction application built using an Artificial Neural Network (ANN) model. The application is deployed using Streamlit and allows users to input customer information to predict the likelihood of churn.

## 🎯 Features

- 🧠 Deep learning model for accurate churn prediction
- 🔄 Interactive Streamlit web interface
- 📊 Real-time prediction visualization
- 🔢 Support for numerical and categorical features
- 📈 Probability score for churn prediction

## 🚀 Demo

![Churn Prediction App Demo](assets/demo.gif)

## 🛠️ Requirements

- Python 3.8+
- TensorFlow 2.x
- Streamlit
- NumPy
- Pandas
- scikit-learn

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ANN-Classification-Churn.git
cd ANN-Classification-Churn
```

2. Create and activate a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## 📝 Usage

1. Make sure you have the required model and encoder files:
   - `model.h5` - The trained TensorFlow model
   - `label_encoder_gender.pkl` - Label encoder for gender
   - `onehot_encoder_geo.pkl` - One-hot encoder for geography
   - `scaler.pkl` - StandardScaler for numerical features

2. Run the Streamlit app:
```bash
streamlit run app.py
```

3. Access the web application at `http://localhost:8501`

## 💻 How It Works

1. User inputs customer information through the interactive Streamlit interface
2. The application preprocesses the data using the saved encoders and scaler
3. The preprocessed data is fed into the trained neural network model
4. The model returns a churn probability
5. The result is displayed to the user with an interpretation

## 🧪 Model Architecture

The model is a neural network built with TensorFlow with the following architecture:
- Input layer matching the number of features
- Multiple hidden layers with ReLU activation
- Output layer with sigmoid activation for binary classification
- Trained using binary cross-entropy loss and Adam optimizer

## 📊 Input Features

- 🌍 Geography: Customer's country of residence
- 👤 Gender: Customer's gender
- 🔢 Age: Customer's age
- 💰 Balance: Account balance
- 💳 Credit Score: Customer's credit score
- 💵 Estimated Salary: Customer's estimated salary
- ⏳ Tenure: Number of years the customer has been with the bank
- 🛒 Number of Products: Number of bank products the customer uses
- 💳 Has Credit Card: Whether the customer has a credit card (0=No, 1=Yes)
- 🏃 Is Active Member: Whether the customer is an active member (0=No, 1=Yes)

## 📈 Output

- Churn Probability: A value between 0 and 1 indicating the likelihood of churn
- Prediction: Interpretation of whether the customer is likely to churn or not

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- TensorFlow team for the amazing deep learning framework
- Streamlit team for the intuitive web app framework
- scikit-learn contributors for the preprocessing tools
