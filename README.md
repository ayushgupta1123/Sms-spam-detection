📩 SMS Spam Classifier

A machine learning web app that classifies SMS messages as Spam or Not Spam, built with Streamlit and scikit-learn.

🔗 Live Demo: []


🧠 Overview

This project uses Natural Language Processing (NLP) to analyze the content of an SMS message and predict whether it is spam or a legitimate ("ham") message. Text is cleaned and transformed using tokenization, stopword removal, and stemming, then converted into numerical features with a TF-IDF vectorizer before being fed into a trained classification model.


✨ Features


Simple, interactive web interface built with Streamlit
Real-time spam prediction for any SMS/text input
NLP preprocessing pipeline: lowercasing, tokenization, stopword & punctuation removal, stemming
Pre-trained TF-IDF vectorizer, feature scaler, and classification model included



🛠️ Tech Stack


Python
Streamlit – web app framework
scikit-learn – model training & inference
NLTK – text preprocessing (tokenization, stopwords, stemming)
Pandas



📂 Project Structure

Sms-spam-detection/
│
├── app.py              # Streamlit application
├── model.pkl           # Trained classification model
├── vectorizer.pkl      # TF-IDF vectorizer
├── scaler.pkl          # Feature scaler
└── requirements.txt    # Python dependencies


⚙️ How It Works


Input – User enters an SMS message in the text area.
Preprocessing – The message is lowercased, tokenized, stripped of stopwords/punctuation, and stemmed using NLTK's Porter Stemmer.
Vectorization – The cleaned text is transformed into numerical features using the pre-fitted TF-IDF vectorizer.
Scaling – Features are scaled using the pre-fitted scaler.
Prediction – The trained model predicts whether the message is spam (1) or not spam (0).
Output – The result is displayed as 🚫 Spam or ✅ Not Spam.



🚀 Getting Started

Prerequisites


Python 3.8+


Installation


Clone the repository


bash   git clone https://github.com/ayushgupta1123/Sms-spam-detection.git
   cd Sms-spam-detection


Install dependencies


bash   pip install -r requirements.txt


Run the app


bash   streamlit run app.py


Open the local URL shown in your terminal (usually http://localhost:8501) in your browser.



Note: On first run, the app automatically downloads the required NLTK data (punkt, punkt_tab, stopwords).




🖥️ Usage


Launch the app.
Enter or paste an SMS message into the text box.
Click Predict.
View the result — Spam or Not Spam.



📦 Deployment

This app is built with Streamlit and can be deployed on:


Streamlit Community Cloud
Render / Railway / Heroku
Docker + any cloud provider


Once deployed, add your live app link at the top of this README.


🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to open a pull request or an issue.


📄 License

This project is open source. Add a LICENSE file to specify usage terms.


👤 Author

Ayush Gupta
GitHub: @ayushgupta1123
