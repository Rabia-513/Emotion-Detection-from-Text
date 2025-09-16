# Emotion-Detection-from-Text
Topic:
 Multi-Class Emotion Detection from Text

1. Project Title
Multi-Class Emotion Detection from Text

2. Purpose of the Project
The goal of this project is to move beyond simple sentiment classification (positive/negative) and accurately identify specific emotions expressed in text. These include:
•	😊 Happy
•	😢 Sad
•	😠 Angry
•	😨 Fear
•	😲 Surprise
•	😐 Neutral

3. Real-World Examples
•	Facebook AI detects harmful emotional content to prevent crises.
•	Replika AI Chatbot adjusts tone and responses based on emotional input.
•	Customer Support Systems use emotional tone to prioritize critical tickets.

4. Dataset
We used an open-source dataset:
•	Crowdflower Emotion Dataset
o	CSV format

o	Contains user-generated text labeled with one of six emotions: Happy, Sad, Angry, Fear, Surprise, Neutral.
 
5. Methodology
Step 1: Data Preprocessing
•	Removed punctuation, numbers, and URLs
•	Converted text to lowercase
•	Applied whitespace normalization
•	Cleaned and tokenized each sentence
 
Step 2: Feature Extraction
•	Used TF-IDF Vectorization to convert text into numerical vectors
•	Max features = 5000
•	Removed English stopwords
 
Step 3: Model Building
•	Baseline Model: Multinomial Naive Bayes (MNB)
•	Trained on 80% of the data, tested on 20%
•	Model was trained for multi-class classification
Step 4: Evaluation
•	Evaluated using:
o	Confusion Matrix
o	Classification Report
	Precision
	Recall
	F1-score (per emotion)
	Macro and Weighted Average F1
•	Achieved overall accuracy of 73%
 
6. Real-time Prediction System
We built a real-time inference tool using Streamlit, which includes:
 
•	 Text Input Box:
 
•	 Emotion Detection with Emoji:
 
•	Confidence Score Bar Chart:
 
•	 Sentiment vs Emotion Comparison:
 
•	Word Clouds per Emotion:
 

7. Bonus Features
 Sentiment vs Emotion Analysis
Used TextBlob to compare sentiment polarity (positive/negative/neutral) against predicted emotions.
 Word Cloud Generation
Automatically generated word clouds for each emotion category to visualize commonly used terms.
 Timeline Trend (Optional)
Feature implemented but hidden when dataset lacks a timestamp column.



8. Conclusion
This project successfully demonstrates a practical multi-class emotion classification system from text using classical machine learning techniques. The system can be further enhanced by incorporating richer datasets, deep learning models, and real-time deployment in production-level environments.

