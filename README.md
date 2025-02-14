# Consumer-Trust-Review-Analysis

# Amazon Fine Food Reviews Analysis

## Introduction
This project aims to analyze consumer trust in online reviews within the digital marketing and consumer behavior sectors, specifically focusing on the Amazon Fine Food Reviews dataset. The primary goal is to perform sentiment analysis to distinguish between trusted and suspicious reviews, providing insights into factors that influence consumer perceptions and buying decisions.

## Project Objectives
- **To analyze the sentiment expressed in the reviews.**
- **To identify key factors that contribute to the trustworthiness of online reviews.**
- **To build a machine learning model to classify reviews as trusted or suspicious.**

## Technologies Used
- **Python**: Main programming language.
- **Pandas & NumPy**: For data manipulation.
- **Matplotlib & Seaborn**: For data visualization.
- **XGBoost**: For building the machine learning model.
- **Scikit-learn**: For model evaluation and additional machine learning tasks.

## Dataset Description
The dataset contains over 500,000 reviews of fine foods from Amazon. Each review includes information such as:
- `ProductId` - ID of the reviewed product.
- `UserId` - ID of the reviewer.
- `ProfileName` - Name of the reviewer.
- `HelpfulnessNumerator` - Number of users who found the review helpful.
- `HelpfulnessDenominator` - Number of users who indicated whether they found the review helpful.
- `Score` - Rating between 1 and 5.
- `Time` - Timestamp of the review.
- `Summary` - Brief summary of the review.
- `Text` - Text of the review.

## Methodology
### Data Preprocessing
- **Cleaning**: Removed duplicates and handled missing data.
- **Transformation**: Extracted features from the text using natural language processing techniques.

### Feature Engineering
- **Text Analysis**: Utilized techniques such as TF-IDF for text representation.
- **Sentiment Analysis**: Used NLP tools to derive sentiment scores from the review texts.

### Model Building
- **XGBoost Classifier**: Chosen for its performance and flexibility. Configured with hyperparameters optimized through cross-validation.

### Model Evaluation
- **Accuracy**: Used as the primary metric to assess the model.
- **Precision, Recall, and F1-Score**: Evaluated to understand the model's performance across classes.

## Results
The analysis revealed significant insights into what makes a review trustworthy. The XGBoost model achieved an accuracy of 69%, with detailed metrics available in the notebook for precision, recall, and F1-scores.

## Visualizations
Included various plots to visualize data distributions. These visualizations are crucial for understanding the data.

## Conclusion and Future Work
This project underscores the importance of understanding consumer trust in online reviews. Future enhancements could include testing other machine learning models, incorporating more complex NLP techniques, or expanding the dataset with additional review sources.


