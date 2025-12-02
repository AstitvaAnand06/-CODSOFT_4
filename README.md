📡 SMS Spam Detection using Machine Learning & Tkinter GUI

A machine learning project that detects whether an SMS message is Spam or Ham (Legitimate) using TF-IDF features and multiple ML classifiers.
The final deployed model uses Support Vector Machine (SVM) with 97.9% accuracy.

📌 Features

📥 Load & preprocess the SMS Spam Collection Dataset

🔤 Text cleaning (lowercasing, removing special characters, whitespace normalization)

🧠 Models Trained:

Multinomial Naive Bayes

Logistic Regression

Support Vector Machine (SVM)

📊 Accuracy and classification report printed for each model

💾 Save the best model (SVM) using joblib

🖥️ Full Tkinter GUI for user input & result display

🎨 Styled UI with coloured output boxes (Green = HAM, Red = SPAM)

📂 Project Structure
├── svm_model.pkl
├── tfidf_vectorizer.pkl
├── spam.csv
├── spam_detector.py   (your main python code)
└── README.md          (this file)

🧠 Machine Learning Pipeline

Load Dataset (Spam/Ham SMS)

Preprocess text → clean, normalize

Convert text to TF-IDF vectors

Train 3 models

Naive Bayes

Logistic Regression

SVM

Evaluate accuracy

Save the best model (SVM)

Use model in Tkinter GUI

🎯 Model Performance (Sample Output)
Model	Accuracy
Naive Bayes (NB)	96–97%
Logistic Regression	96%
SVM (Final Model)	97.9%

SVM performs best because it handles high-dimensional TF-IDF vectors extremely well.

🖥️ GUI Preview

User types a message

Model predicts whether SPAM or HAM

Result is shown in a styled colour box (Red = SPAM, Green = HAM)

▶️ How to Run the Project
1. Install Required Libraries
pip install pandas scikit-learn joblib tkinter

2. Download the Dataset

Dataset link:
https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset

Place spam.csv in your project folder.

3. Run the Application
python spam_detector.py

🧪 Example Predictions

Input:

Congratulations! You've won $1000 cash. Click the link now.


Output:
🟥 Spam Detected!

Input:

Bro, send me your notes please.


Output:
🟩 Ham Message

🛠️ Technologies Used

Python

scikit-learn

Tkinter

TF-IDF Vectorizer

SVM Classifier

Joblib
