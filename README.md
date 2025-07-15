# twitter-sentiment-analysis
# Twitter Sentiment Analysis using VADER

This project performs sentiment analysis on a Twitter dataset to classify tweets into **positive**, **neutral**, or **negative** sentiments. It uses VADER (Valence Aware Dictionary and sEntiment Reasoner), a rule-based sentiment analysis tool optimized for social media text.

---

## 📌 Project Objectives

- Clean and preprocess raw tweet text.
- Use the VADER sentiment analyzer to classify sentiment.
- Compare predicted sentiment with actual labeled sentiment.
- Evaluate performance using classification metrics and a confusion matrix.
- Save results and push them to a GitHub repository.

---

## 📁 Dataset

- **Source**: [Kaggle – Twitter Sentiment Dataset](https://www.kaggle.com/datasets/saurabhshahane/twitter-sentiment-dataset)
- **Format**: ZIP file containing CSV files
- **Features**:
  - `clean_text`: Preprocessed tweet text
  - `category`: Actual sentiment label (positive, neutral, negative)

---

## 🧪 Steps Performed

### ✅ Step 1: Clone GitHub Repository
Used Google Colab to clone this GitHub repo and link with Git for version control.

### ✅ Step 2: Download & Extract Dataset
Downloaded the dataset using `kagglehub` and extracted it from the ZIP file.

### ✅ Step 3: Load Data
Loaded the dataset into a Pandas DataFrame for analysis.

### ✅ Step 4: Preprocess Tweet Text
Performed the following operations:
- Removed mentions (@user), hashtags, URLs, and punctuation
- Lowercased the text
- Removed stopwords
- Tokenized and lemmatized words

### ✅ Step 5: Sentiment Classification with VADER
- Applied VADER to generate sentiment scores for each tweet
- Assigned sentiment labels based on VADER compound score

### ✅ Step 6: Evaluation
- Generated classification report (precision, recall, F1-score)
- Created a confusion matrix to visualize model performance

### ✅ Step 7: Save & Push to GitHub
Saved predictions to `twitter_sentiment_results.csv` and pushed the file to this GitHub repository.

---

## 📊 Results

### Classification Report (Sample)
          precision    recall  f1-score   support

negative       0.72      0.69      0.70       500
 neutral       0.65      0.68      0.66       450
positive       0.78      0.75      0.76       550

accuracy                           0.71      1500
