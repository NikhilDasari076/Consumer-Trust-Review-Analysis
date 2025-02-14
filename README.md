
# Amazon Fine Food Reviews Analysis

## Introduction
This project aims to analyze over 500,000 Amazon fine food reviews to explore consumer trust in online reviews. Using **Natural Language Processing (NLP)** and **Machine Learning**, the goal is to classify reviews as **trusted** or **suspicious** and provide business insights into what influences consumer perceptions of trust.

## Objectives
- Perform **Sentiment Analysis** to extract consumer opinions from review text.
- Identify **trusted vs. suspicious reviews** using predictive modeling.
- Generate insights into factors that influence review trustworthiness.
- Develop a **classification model** to predict the trustworthiness of reviews.

---

## Dataset Description
The dataset contains over **568,000 reviews** of fine foods from Amazon, with the following key fields:
- **ProductId**: Unique identifier for the product.
- **UserId**: Unique identifier for the reviewer.
- **Score**: Rating given by the reviewer (1–5).
- **HelpfulnessNumerator / HelpfulnessDenominator**: Measure of how helpful the review was.
- **Time**: Timestamp of the review.
- **Summary**: Short summary of the review.
- **Text**: Full text of the review.

  ## Dataset : https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews


---

## Technologies and Tools Used
- **Languages**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, NLTK, Scikit-learn, XGBoost
- **Machine Learning**: XGBoost Classifier for prediction
- **Natural Language Processing (NLP)**: Sentiment analysis using TextBlob and feature extraction using TF-IDF
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score

---

## Methodology
### **1. Data Preprocessing**
- Removed duplicates and handled missing values.
- Converted review timestamps into datetime format.
- Engineered features like **review length** and **helpfulness ratio**.

### **2. Sentiment Analysis**
- Extracted sentiment polarity scores from the review text to quantify positive or negative sentiments.

### **3. Feature Engineering**
- Applied **TF-IDF Vectorization** to transform review text into numerical features for machine learning.
- Combined structured features (e.g., sentiment score, review length) with text-based features.

### **4. Machine Learning**
- Built an **XGBoost Classifier** to predict whether a review is trusted or suspicious.
- Evaluated model performance using Accuracy, Precision, Recall, and F1-score.

---

## Model Performance
The **XGBoost Classifier** achieved the following results on the test set:

- **Accuracy**: 68.8%
- **Class 0 (Not Trusted Reviews)**:
  - Precision: 0.65
  - Recall: 0.83
  - F1-Score: 0.73
- **Class 1 (Trusted Reviews)**:
  - Precision: 0.76
  - Recall: 0.55
  - F1-Score: 0.64

### **Insights from the Model:**
- **Helpfulness ratio** and **sentiment polarity** were key factors in identifying trusted reviews.
- Reviews with extremely high or low ratings (1 or 5 stars) often had a lower trustworthiness score.
- **Longer reviews** were more likely to be perceived as trusted compared to shorter ones.

---

## Visualizations
Key visualizations generated during the analysis include:
1. **Distribution of Ratings (1-5 Stars)**
2. **Helpfulness Ratio Distribution**
3. **Sentiment Score Trends Over Time**
4. **Review Length vs. Helpfulness Ratio**

---

## Insights and Business Impact
- Businesses can use this analysis to filter suspicious reviews and improve their online reputation.
- Sentiment analysis provides valuable insights into consumer opinions, enabling better product improvements.
- Helps consumers make more informed decisions by highlighting trusted reviews.

---









