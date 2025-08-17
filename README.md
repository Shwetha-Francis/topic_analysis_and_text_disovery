# topic_analysis_and_text_disovery
# Text Analysis Project

## Overview
This project analyzes a set of documents to extract insights using three main techniques:
1. **TF-IDF**: Identifies the most important words in each document.
2. **Word2Vec**: Captures semantic similarity between words.
3. **LDA (Latent Dirichlet Allocation)**: Discovers hidden topics across all documents.

---

## Dataset
The dataset consists of 12 sample text documents including topics like electronics, entertainment, food, and travel.  
Each document contains sentences describing products, experiences, or events.

---

## Preprocessing
Before analysis, the text undergoes:
- Lowercasing
- Removing punctuation and numbers
- Removing stopwords (common English words)
- Tokenization into words

Example:

| Original Text | Tokens |
|---------------|--------|
| The phone has great battery life and an amazing camera. | ['phone', 'great', 'battery', 'life', 'camera'] |

---

## TF-IDF Analysis
- Highlights important words per document.
- Example top words:

| Document | Top Words |
|----------|-----------|
| 1        | phone, battery, camera, life, great |
| 3        | movie, action, exciting, scenes, full |

- Indicates document-specific focus.

---

## Word2Vec Analysis
- Captures semantic similarity between words.
- Example:

| Word   | Top 5 Similar Words |
|--------|-------------------|
| phone  | camera, smartwatch, laptop, battery, device |
| movie  | concert, action, plot, scenes, game |
| food   | restaurant, delicious, meal, affordable, service |

- Helps find related concepts across documents.

---

## LDA Topic Modeling
- Discovers hidden topics in the corpus.
- Example topics:

| Topic | Top Words |
|-------|-----------|
| 0     | battery, phone, laptop, camera, design |
| 1     | movie, action, concert, plot, music |
| 2     | food, restaurant, delicious, affordable, service |
| 3     | software, game, graphics, buggy, crashes |
| 4     | travel, experience, scenery, beautiful, excellent |

- Helps understand major themes across all documents.

---

## Visualizations
- **TF-IDF**: Bar charts of top words per document (optional).  
- **Word2Vec**: 2D plot of embeddings using PCA or t-SNE (optional).  
- **LDA**: Interactive topic visualization using `pyLDAvis`.

---

## Insights
- TF-IDF identifies unique important words per document.
- Word2Vec captures semantic relationships between words.
- LDA uncovers underlying topics and main themes.
- Dominant themes: Electronics, Entertainment, Food, Travel.

---

## Tools & Libraries
- Python 3.x
- Libraries: `NLTK`, `Gensim`, `scikit-learn`, `pyLDAvis`
- Visualization: Matplotlib (optional), PyLDAvis

---

## How to Run
1. Clone the repository.
2. Install required libraries:
```bash
pip install nltk gensim scikit-learn pyLDAvis
