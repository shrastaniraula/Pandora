# Pandora: NLP Chatbot

## Project Description
Pandora is a simple chatbot built to assist users with mental health conversations using basic NLP techniques. It takes user input, cleans and processes it, and finds the closest matching response from a dataset. The goal is to create a small, text-based chatbot that can recognize common emotional expressions and reply in a supportive way. This project was made to learn and practice NLP concepts like tokenization, lemmatization, and vectorization.

---
## Algorithm Used
Pandora uses TF-IDF vectorization and cosine similarity to find the most relevant response. The dataset contains intents with example phrases and responses. When a user sends a message, the chatbot processes it, converts it into a TF-IDF vector, and compares it with all patterns in the dataset. The response corresponding to the highest similarity score is shown to the user.

---
## How to Run
1. Clone the repository  
   `git clone https://github.com/shrastaniraula/Pandora.git`  
   `cd Pandora`
2. Install dependencies  
   `pip install nltk pandas scikit-learn matplotlib`
3. Download NLTK data  
   `import nltk`
    `nltk.download('stopwords')`
    `nltk.download('wordnet')`
    `nltk.download('averaged_perceptron_tagger')`
4. Run the file  
`python pandora_chatbot.py`

---
## Core NLP Pipeline
1. Punctuation Removal  
2. Stopword Filtering (customized)  
3. Negation Handling  
4. POS Tagging for Important Words  
5. Lemmatization  
6. TF-IDF Vectorization  
7. Cosine Similarity for Response Selection
