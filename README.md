# Healthcare Premium Prediction App

An end-to-end Machine Learning application that predicts health insurance premiums based on user demographics, medical history, and financial status. 

The project utilizes a **dual-model architecture**:
* **Model Young:** Specifically trained for individuals aged 25 and under.
* **Model Rest:** Optimized for individuals over the age of 25.

## 🚀 Features
* **Dynamic Risk Scoring:** Implements a custom normalization logic for medical histories (e.g., combining risks for Diabetes and Heart Disease).
* **Automated Feature Engineering:** Handles One-Hot Encoding for categorical inputs like BMI Category, Smoking Status, and Region.
* **Real-time Scaling:** Uses pre-trained `MinMaxScaler` objects to ensure input data matches the training distribution.
* **Streamlit Interface:** A clean, user-friendly web interface for instant predictions.

## 📁 Project Structure
```text
├── artifacts/               # Saved .joblib models and scalers
├── main.py                  # Streamlit UI code
├── prediction_helper.py     # Preprocessing, Scaling, and Prediction logic
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
```
# Clone the Repository 
git clone [https://github.com/your-username/healthcare-premium-prediction.git](https://github.com/your-username/healthcare-premium-prediction.git)
cd healthcare-premium-prediction
# Setup Bash Environment
python -m venv venv
````
├──Activate on Windows:
├────.\venv\Scripts\activate
├──Activate on Mac/Linux:
├────source venv/bin/activate
````
# Install Dependencies
pip install -r requirements.txt
# Run the App
streamlit run main.py
