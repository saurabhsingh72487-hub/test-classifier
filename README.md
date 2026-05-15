📩 Neural Network SMS Text Classifier
📌 Project Overview

This project builds a Neural Network-based SMS spam classifier that predicts whether a message is ham (normal message) or spam (advertisement/scam message) using machine learning.

It uses a deep learning model built with TensorFlow/Keras and trained on the SMS Spam Collection dataset.
📊 Dataset

The dataset contains SMS messages labeled as:

ham → normal message from friends/family
spam → unwanted advertisements or scams

The dataset is split into:

80% Training data
20% Testing data
⚙️ Technologies Used
Python 🐍
TensorFlow / Keras
TensorFlow Datasets (TFDS)
NumPy
Matplotlib
Tokenization (NLP preprocessing)
🧠 Model Architecture

The neural network includes:

Embedding Layer (text → vector representation)
Global Average Pooling Layer
Dense Layer (24 neurons, ReLU activation)
Output Layer (Sigmoid activation)
🔄 Workflow
Load SMS dataset using TFDS
Convert text into numerical sequences
Tokenize and pad sequences
Build neural network model
Train model on labeled data
Evaluate performance
Predict new messages using function
📌 Prediction Function
predict_message("Free money!!! Claim now!!!")
📤 Output format:
[0.98, "spam"]
First value → probability (0 to 1)
Second value → predicted label ("ham" or "spam")
🎯 Goal

To correctly classify SMS messages with high accuracy and detect spam messages effectively.

📈 Model Performance
Uses binary classification (spam vs ham)
Optimized using Adam optimizer
Loss function: Binary Crossentropy
Accuracy improves with training epochs
🚀 How to Run
Open Google Colab or Jupyter Notebook
Paste the full code
Run all cells sequentially
Test using predict_message() function
📁 Project Structure
sms-spam-classifier/
│
├── sms_classifier.ipynb
├── README.md
└── dataset (loaded via TFDS)
💡 Key Learnings
Natural Language Processing (NLP)
Text tokenization and padding
Neural network for classification
Binary classification using deep learning
Working with TensorFlow Datasets
🔮 Future Improvements
Use LSTM/GRU for better accuracy
Improve preprocessing (stopwords, stemming)
Deploy as web app (Flask / Streamlit)
Add real-time SMS filtering system
👨‍💻 Author

Built as part of Machine Learning Certification Project.
