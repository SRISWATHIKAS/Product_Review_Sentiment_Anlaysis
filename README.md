# Product_Review_Sentiment_Anlaysis
Transformer-based sentiment analysis of product reviews using sentence embeddings and Random Forest classification to identify positive, neutral, and negative customer feedback.

# Product Reviews Sentiment Analysis

## 📌Overview

This project develops a **sentiment analysis system** to classify customer product reviews into three categories:

* 🟢 Positive
* 🟡 Neutral
* 🔴 Negative

The project uses **Transformer-based sentence embeddings** with machine learning classifiers to analyze customer feedback and support data-driven business decisions.

## 🎯 Objective

The main objective is to automatically analyze large volumes of customer reviews and identify their sentiment. This can help businesses understand customer satisfaction, discover areas for improvement, and address negative feedback.

## 📊 Dataset

The dataset contains **1,007 reviews and 3 columns**:

* **Product ID** – Unique identifier for each product
* **Product Review** – Customer feedback and opinions
* **Sentiment** – Positive, Neutral, or Negative

- The dataset is **highly imbalanced**, with approximately **850 positive reviews** and around **75 neutral and 75 negative reviews**.

## 🧠 Methodology

The project follows these main steps:

1. Load and inspect the dataset
2. Clean duplicate records
3. Perform Exploratory Data Analysis (EDA)
4. Generate sentence embeddings using:

   * `all-MiniLM-L6-v2`
5. Split the data into **80% training and 20% testing**
6. Train machine learning models:

   * Random Forest
   * Gradient Boosting
7. Evaluate models using:

   * Accuracy
   * Weighted F1 Score
8. Select the final model based on test performance and generalization

## 🤖 Models Used

### Random Forest + Transformer

* Training Accuracy: **100%**
* Test Accuracy: **86.5%**
* Test F1 Score: **81.8%**

### Gradient Boosting + Transformer

* Training Accuracy: **99.88%**
* Test Accuracy: **84.07%**
* Test F1 Score: **80.3%**

Based on the notebook's model-selection results, **Random Forest + Transformer** was selected as the final model.

## 📈 Evaluation Metrics

- **Accuracy** measures the overall percentage of correct predictions.

- **F1 Score** balances precision and recall and is particularly useful for evaluating performance when sentiment classes are imbalanced.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Sentence Transformers
* Matplotlib
* Seaborn


## ✅ Conclusion

- **Transformer embeddings combined with machine learning** can effectively classify customer reviews into positive, neutral, and negative sentiments. 

- The Random Forest model achieved the strongest test performance among the evaluated approaches and provides a foundation for future improvements and deployment.
