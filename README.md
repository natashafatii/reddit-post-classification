# 📊 Reddit Sentiment Analysis & Topic Classification – NLP Project

[![Python 3.9+](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![NLP](https://img.shields.io/badge/NLP-Sentiment_Analysis-4CAF50)](https://en.wikipedia.org/wiki/Natural_language_processing)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?logo=googlecolab&logoColor=white)](https://colab.research.google.com/)
[![Status](https://img.shields.io/badge/Status-Complete-00C853)]()
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

A complete end-to-end **Natural Language Processing (NLP) pipeline** for sentiment analysis and topic classification of Reddit posts, featuring data collection, preprocessing, modeling, and an interactive Power BI dashboard.

---

## 🔗 Live Dashboard

### 📊 Public Power BI Dashboard
[![Open in Power BI](https://img.shields.io/badge/🚀_View_Live_Dashboard-FF4500?style=for-the-badge&logo=powerbi&logoColor=white)](https://app.powerbi.com/view?r=eyJrIjoiY2JhZjM2NzMtNzUxMS00ZjBjLWFiNGYtZGIwMzU0NDk2NzZlIiwidCI6IjkwMWQ5YTk5LTI3NTgtNGM5ZS1iNWM3LTI2MWM2OTIwZmQzNyIsImMiOjl9)

**Direct Link:**  
`https://app.powerbi.com/view?r=eyJrIjoiY2JhZjM2NzMtNzUxMS00ZjBjLWFiNGYtZGIwMzU0NDk2NzZlIiwidCI6IjkwMWQ5YTk5LTI3NTgtNGM5ZS1iNWM3LTI2MWM2OTIwZmQzNyIsImMiOjl9`

**Dashboard Features:**
- Interactive sentiment filtering (Positive/Neutral/Negative)
- Topic-wise post distribution
- Subreddit comparison charts
- Date-range selectors
- Real-time visual updates
- **Public access – no login required**

---

## 📂 Repository Structure
```
reddit-sentiment-analysis-nlp-project/
├── 📁 data/ # Datasets
│ ├── raw_reddit_data.csv
│ ├── preprocessed_reddit_data.csv
│ ├── reddit_live_data.csv
│ └── classified_reddit_data.csv
├── 📁 notebooks/ # Colab Notebooks
│ └── ids_4.ipynb
├── 📁 dashboard/ # Power BI Assets
│ └── ids_4.pbix
├── PROJECT_SUMMARY_REPORT.pdf
└── README.md # This File
```
---

## 🧠 Project Workflow

### 1. **Data Collection**  
- **Tool:** PRAW (Python Reddit API Wrapper)  
- **Subreddits:** `r/technology`, `r/mentalhealth`, `r/AskReddit`  
- **Volume:** 60 posts (20 per subreddit)  
- **Fields:** Title, body, author, score, comment count, timestamp  

### 2. **Text Preprocessing**  
- Lowercasing, punctuation/URL/mention removal  
- Custom Reddit stopword list + NLTK stopwords  
- Tokenization & text normalization  

### 3. **Sentiment Analysis**  
- **Models:** VADER (rule-based) + TextBlob (lexicon-based)  
- **Labels:** Positive (😊), Neutral (😐), Negative (😔)  
- **Agreement Rate:** 85% between models  

### 4. **Topic Classification**  
- Keyword-based classification into 5 topics:  
  - Technology, Mental Health, Education, Entertainment, Politics  
- Manual validation for accuracy assurance  

### 5. **Dashboard & Visualization**  
- Built in Power BI with interactive visuals  
- Published to Power BI Service for public access  
- Supports filtering by sentiment, topic, date, and subreddit  

---

## 📈 Key Results

| Metric | Result | Insight |
|--------|--------|---------|
| Total Posts | 60 | Balanced dataset from 3 subreddits |
| Sentiment Distribution | Positive: 42% | Generally positive discourse |
| Model Agreement | 85% | High reliability between VADER & TextBlob |
| Dominant Topic | Technology | Most frequent in collected data |
| Dashboard Availability | Public | Accessible without authentication |
| Data Cleaned | 25–40% reduction | Effective preprocessing |

---

## 🛠️ Tech Stack

| Layer | Technology | Use Case |
|-------|------------|----------|
| **Language** | Python 3.9+ | Core programming |
| **Data Collection** | PRAW | Reddit API integration |
| **NLP Libraries** | NLTK, TextBlob, VADER | Sentiment & text processing |
| **Data Processing** | Pandas, NumPy | Data manipulation |
| **Visualization** | Power BI, Matplotlib | Dashboards & plots |
| **Development** | Jupyter, Google Colab | Interactive coding |
| **Version Control** | Git, GitHub | Collaboration & tracking |

---

## 🚀 Quick Start

### Prerequisites
- Python 3.9+
- Reddit API credentials (for data collection)
- Power BI Desktop (optional, for editing `.pbix`)

### Installation
```bash
# Clone repository
git clone https://github.com/natashafatii/reddit-post-classification.git
cd reddit-post-classification

# Create virtual environment (optional)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your Reddit API credentials
