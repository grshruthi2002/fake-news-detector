# Truth Seeker: Multimodal Fake News Detection System

## Project Objective
The rapid spread of misinformation through both text and manipulated images poses a significant threat to public trust and decision-making[cite: 11, 19, 20].The objective of this project is to build a dual-modal "Truth Seeker" system capable of detecting fake news in real-time[cite: 1, 2, 15]. [cite_start]The system evaluates both textual claims and visual content independently to verify the authenticity of news articles[cite: 12, 13, 14].

## Frameworks & Libraries
- [cite_start]**Programming & Backend:** Python, Flask [cite: 15]
- [cite_start]**Machine Learning (Text):** Scikit-Learn (TF-IDF, Passive Aggressive Classifier, Naive Bayes, SVM) [cite: 13, 25]
- [cite_start]**Deep Learning (Images):** Convolutional Neural Networks (CNN), Vision Transformer (ViT-B/16) [cite: 12, 14, 25]
- [cite_start]**Frontend:** HTML/CSS [cite: 100]

## System Architecture
[cite_start]The application features an integrated web interface that allows users to upload text or images for instant classification, while also categorizing the news into domains like Politics, Weather, and Sports[cite: 15, 27, 97].

**1. Text-Based Detection Pipeline**
- [cite_start]Takes raw news text as input and converts it into numerical vectors using TF-IDF[cite: 64].
- [cite_start]Utilizes a Passive Aggressive Classifier integrated with a hybrid model (Naive Bayes, SVM, CNN) to classify text as Real or Fake[cite: 65]. 

**2. Image-Based Detection Pipeline**
- [cite_start]Processes uploaded news images, memes, or posters[cite: 83, 87].
- [cite_start]Leverages a fine-tuned Vision Transformer (ViT-B/16) to extract deep feature representations and perform binary classification (Real vs. Fake)[cite: 84, 86].

## Performance & Insights
The model was rigorously evaluated and demonstrated high reliability across both modalities:
- [cite_start]**High Accuracy:** The system achieved a 98.8% training accuracy and a 97% testing accuracy over 10 epochs[cite: 214].
- [cite_start]**Strong Classification Metrics:** Precision, recall, and F1-score all exceeded 0.94, indicating a well-balanced model[cite: 216].
- [cite_start]**Low Misclassification:** The confusion matrix revealed only 8 misclassifications out of 240 samples evaluated[cite: 215].
- [cite_start]**Image Model Superiority:** The CNN-based visual model achieved 94.5% accuracy, outperforming baselines like Naive Bayes (83%) and SVM (94%)[cite: 218].

## Publication Status
- [cite_start]**Conference:** International Conference on Computing Technologies (ICOCT 2025) [cite: 235]
- [cite_start]**Status:** Paper Communicated [cite: 234]

## Web Application Previews
The system provides a real-time Flask web interface, allowing users to upload articles or images and instantly receive a classification of "Real" or "Fake" News.

![Fake News Detector Interface](https://github.com/grshruthi2002/Hybrid-CNN-Fake-News-Detector/blob/main/ouput_screenshot_%20Multimodal%20Fake%20News%20Detection%20System.png?raw=true)
