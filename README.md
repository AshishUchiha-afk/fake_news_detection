#  📰 fake_news_detection
A machine learning model to detect fake news articles using natural language processing and classification techniques.

## ⚙️ How to Run the Code Without Hassle in google colab

Follow the steps below to get started easily:

1. 📥 **Run the following cell in the notebook:**

   ```python
   from google.colab import files
   files.upload()
2.🔐 Upload your Kaggle token (kaggle.json) when prompted.

3.✅ Now the code is ready to run — all necessary permissions and access will be set up!

## ⚙️ How to Set Up the Project Locally (Kaggle API Method)

Follow these steps if you want to use the Kaggle API to download the dataset directly:

1. 🔑 **Get Your Kaggle API Credentials**  
   - Go to your [Kaggle Account Settings](https://www.kaggle.com/account)
   - Click on **"Create New API Token"**
   - This will download a file called `kaggle.json`

2. 📁 **Place the Token File**  
   - Move `kaggle.json` to the `.kaggle` folder:
     - On Windows: `C:\Users\<YourUsername>\.kaggle\kaggle.json`
     - On macOS/Linux: `~/.kaggle/kaggle.json`

3. 🧠 **Use the Following Code to Programmatically Download the Dataset**

   ```python
   import os
   import kaggle

   # Set Kaggle credentials (optional if kaggle.json is correctly placed)
   os.environ['KAGGLE_USERNAME'] = 'your_username'
   os.environ['KAGGLE_KEY'] = 'your_key'

   # Download and unzip the dataset
   kaggle.api.dataset_download_files('dataset', path='.', unzip=True)

---
## 📌 Project Highlights

- 🧠 Binary classification: **Fake (1)** or **Real (0)**
- 📊 Data preprocessing with tokenization, stopword removal, and TF-IDF vectorization
- 🔍 Trained using models like Logistic Regression, Naive Bayes, or PassiveAggressiveClassifier
- 📈 Evaluates performance using accuracy, confusion matrix, and classification report
- 💾 Saves the final model using Pickle for future predictions

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- NLTK / re (Regex) for preprocessing
- TF-IDF Vectorizer
- Pickle

---

## 📁 Project Structure

Fake_News_Detection/
├── fake_news_detection.ipynb → Main notebook
├── fake.csv → Dataset file
├── fake_news_model.pkl → Saved trained model
├── vectorizer.pkl → Saved TF-IDF vectorizer
└── README.md → Project documentation

## 🧪 Example Features Used

- Article title/text
- Word frequency and TF-IDF features

---

## 📈 Evaluation Metrics

- Accuracy Score
- Confusion Matrix
- Classification Report

---

## 📌 Future Improvements

- Add Streamlit or Flask web interface for real-time news input
- Use deep learning models like LSTM or BERT
- Deploy via web or API

---
