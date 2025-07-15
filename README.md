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


### Confusion Matrix

|              | Predicted Negative | Predicted Neutral | Predicted Positive |
|--------------|--------------------|-------------------|--------------------|
| Actual Negative | 345 | 89 | 66 |
| Actual Neutral  | 64 | 305 | 81 |
| Actual Positive | 42 | 95 | 413 |

---

## 🛠️ Technologies Used

- **Python 3**
- **Google Colab**
- **Pandas**, **NumPy**
- **NLTK** – Stopwords, Tokenizer, VADER
- **Matplotlib**, **Seaborn** – Visualization
- **Scikit-learn** – Evaluation metrics
- **Git + GitHub** – Version control

---

## 📈 Visualizations (Optional)

- Confusion matrix heatmap
- Pie chart or bar plot of sentiment distribution
- Word cloud of most frequent words per sentiment (can be added later)

---

## 📥 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Vikram7447/twitter-sentiment-analysis.git
   cd twitter-sentiment-analysis

