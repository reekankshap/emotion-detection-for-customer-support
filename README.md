# 🎭 Emotion Detection for Customer Support – AI-Powered Ticket Generator

## 📌 Overview

The **Emotion Detection for Customer Support** system is an AI-powered application that analyzes customer reviews and automatically detects emotions from textual feedback. Based on the predicted emotion, the system generates support tickets and assigns priority levels for faster issue resolution.

This project helps organizations:
- Identify dissatisfied customers quickly
- Automate complaint management
- Improve customer support efficiency
- Reduce manual review analysis
- Prioritize emotionally critical feedback in real-time

---

## 🎯 Key Features

- Multi-Model Training (Logistic Regression, Random Forest, Naive Bayes)
- Emotion Classification using Machine Learning
- Automated Ticket Generation
- Priority Assignment for Critical Reviews
- Real-Time Emotion Prediction
- TF-IDF Feature Engineering
- High Accuracy Prediction System

---

## 📂 Project Structure

```bash
emotion-detection-for-customer-support/
│
├── customer_emotion_detector.ipynb
├── dataset.csv
├── emotion_model.pkl
├── vectorizer.pkl
├── trained_ai_tickets.csv
├── requirements.txt
└── README.md
```

---

## 🧠 Machine Learning Models Used

The project trains and compares multiple machine learning algorithms to identify the best-performing model.

### Models Implemented

- Logistic Regression
- Random Forest Classifier
- Multinomial Naive Bayes

### Model Performance

| Model | Accuracy |
|---|---|
| Logistic Regression | 86.44% |
| Random Forest | 85.34% |
| Naive Bayes | 85.98% |

The Logistic Regression model achieved the highest accuracy and was selected as the final model.

---

## 📊 Dataset Information

The dataset contains customer reviews labeled with emotional categories.

### Emotion Categories

- Joy / Happy
- Neutral
- Anger / Sadness

### Example Dataset

| Customer Review | Emotion |
|---|---|
| Amazing customer support! | Joy |
| The product quality is average. | Neutral |
| Worst experience ever. | Anger/Sadness |

---

## ⚙️ System Workflow

### 1. Data Collection
Customer reviews are collected and stored in CSV format.

### 2. Data Preprocessing
Text data cleaning includes:
- Lowercasing
- Punctuation removal
- Stopword removal
- Handling empty reviews

### 3. Feature Engineering

TF-IDF Vectorization converts customer reviews into numerical vectors.

```python
TfidfVectorizer(max_features=5000, ngram_range=(1,2))
```

### 4. Model Training
Multiple machine learning models are trained and evaluated using Scikit-learn.

### 5. Emotion Prediction
The trained model predicts emotions for new customer reviews.

### 6. Automated Ticket Generation
Negative and neutral reviews automatically generate support tickets with assigned priority levels.

---

## 💻 Interactive Emotion Testing

Users can manually enter customer reviews for real-time emotion prediction.

### Example Input

```text
"The support team ignored my complaint completely."
```

### Example Output

```text
Predicted Emotion: Anger/Sadness
Confidence Score: 94%
Priority Level: High
Ticket Generated Successfully
```

---

## 🔧 Installation and Setup

### Clone Repository

```bash
git clone https://github.com/reekankshap/emotion-detection-for-customer-support.git
```

### Navigate to Project Folder

```bash
cd emotion-detection-for-customer-support
```

### Install Required Libraries

```bash
pip install -r requirements.txt
```

### Run Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
customer_emotion_detector.ipynb
```
## 🌐 Run Localhost Frontend

If using a Flask frontend:

```bash
python app.py
```

Then open:

```text
http://127.0.0.1:5000/
```

---

## 📦 Required Libraries

```text
pandas
numpy
scikit-learn
matplotlib
joblib
```

---

## 📈 Results

The system successfully classifies customer emotions and generates support tickets automatically for emotionally sensitive reviews.

### Key Achievements

- Accurate emotion classification
- Automated support prioritization
- Intelligent ticket generation
- Real-time customer feedback analysis
- Improved complaint handling workflow

---

## 🌟 Applications

- Customer Support Automation
- Complaint Management Systems
- AI-Based Help Desk Systems
- Review Analysis Platforms
- Customer Feedback Monitoring
- Sentiment-Aware Ticketing Systems

---

## 🚀 Future Enhancements

- Deep Learning using BERT
- Real-time dashboard deployment
- Flask/Streamlit web application
- Email and SMS notifications
- Multi-language emotion detection
- Voice-based sentiment analysis
- CRM integration

---

## 🤝 Contributing

Contributions are welcome.

If you would like to contribute:
1. Fork the repository
2. Create a new feature branch
3. Commit your changes
4. Submit a pull request

Suggestions and improvements are always appreciated.

---

## 🐛 Issues and Bug Reports

If you encounter any bugs or issues while running the project, feel free to open an issue in the repository.

Please include:
- Error description
- Steps to reproduce the issue
- Screenshots (if applicable)

---

## 📜 License

This project is developed for educational and learning purposes.

---

## 👩‍💻 Author

**Reekanksha Prakash**

---

## 📬 Contact

- GitHub: https://github.com/reekankshap
- LinkedIn: https://www.linkedin.com/in/reekanksha-prakash-6ba5b8259
- Email: reekankshaprakash@gmail.com
