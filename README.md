# SMS Spam Detection using NLP

Classifies an SMS message (text input) as **spam** or **ham** (not spam).

## Dataset
[SMS Spam Collection Dataset (Kaggle)](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset) - about 5,500 labeled English SMS messages.
Download `spam.csv` and place it in the `data/` folder.

## Approach
1. Remove duplicates and encode labels (ham = 0, spam = 1)
2. Text preprocessing: lowercase, remove punctuation/numbers and stopwords, stemming (NLTK)
3. Feature extraction: TF-IDF (unigrams + bigrams, 3000 features)
4. Models: Multinomial Naive Bayes and Logistic Regression
5. Evaluation: accuracy, precision, recall, F1, confusion matrix (the data is imbalanced, so accuracy alone is not enough)

## Results
| Model | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| Naive Bayes | XX | XX | XX | XX |
| Logistic Regression | XX | XX | XX | XX |

_(Replace XX with your own results after running.)_

## Run it
```bash
pip install -r requirements.txt
python spam_detection.py --data data/spam.csv
```

Colab notebook: https://colab.research.google.com/drive/13H2NI_L1WupftvFthQpZaHAVwpykMzpU?usp=sharing

## Tech stack
Python, pandas, NLTK, scikit-learn, matplotlib, seaborn
