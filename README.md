# Big-Data-and-Applied-Data-Analytics
Sentiment Analysis on IMDb Movie Reviews
# 🎬 IMDb Sentiment Analysis: Big Data Pipeline

![Apache Spark](https://img.shields.io/badge/Apache%20Spark-PySpark-E25A1C.svg)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248.svg)
![NLP](https://img.shields.io/badge/NLP-Sentiment%20Analysis-blue.svg)
![Institution](https://img.shields.io/badge/Institution-Beykoz%20University-red.svg)

## 📖 Overview
This repository contains an end-to-end Big Data pipeline designed to perform scalable sentiment classification on a massive dataset of IMDb movie reviews. Developed for the *Advanced Big Data and Applied Data Analytics* course, this project demonstrates the integration of distributed computing with cloud-native NoSQL storage to solve modern Natural Language Processing (NLP) challenges.

The system efficiently ingests, processes, and classifies 50,000 movie reviews into positive or negative sentiments, archiving the predictive results and model metrics in the cloud for real-time monitoring.

## ⚙️ Technical Architecture
The project moves beyond local execution environments, adopting a robust cloud-native and distributed computing architecture:
* **Distributed Processing:** **PySpark** is utilized to handle large-scale data transformations, feature extraction, and machine learning efficiently across clusters.
* **Cloud-Native Storage:** **MongoDB Atlas** serves as the persistent NoSQL data layer for both initial data ingestion and the final storage of predictions.
* **Machine Learning:** Implements **Logistic Regression** trained on 10,000 extracted text features to perform accurate binary sentiment classification.

## 🚀 Pipeline Workflow
1. **Massive Data Ingestion:** Automated retrieval of the 50,000-review dataset directly from the MongoDB cloud environment.
2. **Scalable Transformation:** Distributed text preprocessing, tokenization, and feature engineering (yielding 10,000 features) using PySpark's robust NLP capabilities.
3. **Predictive Modeling:** Training and evaluation of the sentiment classifier to distinguish between positive and negative critiques.
4. **Data Persistence:** Pushing the final predictions and model performance metrics back to MongoDB Atlas to ensure no data is lost in temporary memory.

## 🔮 Future Roadmap
While the current architecture successfully handles millions of reviews, planned enhancements include:
* **Deep Learning Integration:** Transitioning from Logistic Regression to **BERT** (Bidirectional Encoder Representations from Transformers) for deeper, context-aware understanding.
* **Feature Expansion:** Scaling the feature vocabulary count from 10,000 to over 50,000 to capture more nuanced language and slang.
* **Real-Time Analysis:** Implementing **Spark Streaming** to analyze and classify live movie review feeds dynamically as they are published.



---
*If you find this Big Data architecture useful, consider giving this repository a ⭐!*
