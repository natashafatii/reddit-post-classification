# 📊 Reddit Sentiment Analysis & Topic Classification - Complete NLP Project

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)
![PowerBI](https://img.shields.io/badge/Power_BI-F2C811?logo=powerbi&logoColor=black)
![NLP](https://img.shields.io/badge/NLP-Sentiment_Analysis-4CAF50)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Colab](https://img.shields.io/badge/Google_Colab-F9AB00?logo=googlecolab&logoColor=white)
![Status](https://img.shields.io/badge/Project-Complete-00C853)
![License](https://img.shields.io/badge/License-MIT-blue)

## 🎯 **Project Overview**

**A comprehensive end-to-end Natural Language Processing (NLP) project** that analyzes Reddit posts to perform sentiment analysis and topic classification. This project demonstrates the complete data science pipeline from data collection to interactive dashboard deployment.

---

## 🚀 **Live Interactive Dashboard**

### **📊 Public Power BI Dashboard**
[![Power BI Live Dashboard](https://img.shields.io/badge/🔗_LIVE_DASHBOARD-FF4500?style=for-the-badge&logo=powerbi&logoColor=white)](https://app.powerbi.com/view?r=eyJrIjoiY2JhZjM2NzMtNzUxMS00ZjBjLWFiNGYtZGIwMzU0NDk2NzZlIiwidCI6IjkwMWQ5YTk5LTI3NTgtNGM5ZS1iNWM3LTI2MWM2OTIwZmQzNyIsImMiOjl9)

**🔗 Direct Link:**  
`https://app.powerbi.com/view?r=eyJrIjoiY2JhZjM2NzMtNzUxMS00ZjBjLWFiNGYtZGIwMzU0NDk2NzZlIiwidCI6IjkwMWQ5YTk5LTI3NTgtNGM5ZS1iNWM3LTI2MWM2OTIwZmQzNyIsImMiOjl9`

**✅ Features:**
- Real-time sentiment filtering
- Interactive topic visualization
- Subreddit comparison
- Date range selection
- **No login required** - Fully public access

---

## 📋 **Project Structure**  
---

## 🎬 **Quick Navigation**

| Section | Content | Files |
|---------|---------|-------|
| **📊 Dashboard** | Live Power BI Dashboard | `dashboard/` |
| **📓 Notebooks** | Complete Jupyter Notebooks | `notebooks/` |
| **📄 Reports** | Project Reports | `reports/` |
| **📁 Data** | All CSV Files | `data/` |
| **🖼️ Screenshots** | Output Visuals | `screenshots/` |
| **🐍 Code** | Python Scripts | `src/` |

---

## 🔍 **Project Workflow**

### **📥 1. Data Collection**
- **Source**: Reddit API via PRAW
- **Subreddits**: r/technology, r/mentalhealth, r/AskReddit
- **Posts Collected**: 60 (20 from each subreddit)
- **Data Extracted**: Title, Body, Author, Upvotes, Comments, Timestamp

**📁 Files:** `notebooks/01_reddit_data_collection.ipynb`, `data/raw_reddit_data.csv`

### **🧹 2. Text Preprocessing**
- Lowercasing & punctuation removal
- URL, mention, hashtag removal
- Stopword removal (NLTK + custom Reddit stopwords)
- Tokenization & text normalization

**📁 Files:** `notebooks/02_text_cleaning_preprocessing.ipynb`, `data/preprocessed_reddit_data.csv`

### **📊 3. Sentiment Analysis**
- **Dual-Model Approach**: VADER + TextBlob
- **Sentiment Labels**: Positive 😊, Neutral 😐, Negative 😔
- **Combination Logic**: Agreement-based decision making
- **Performance**: 85% model agreement rate

**📁 Files:** `notebooks/03_sentiment_topic_classification.ipynb`

### **🏷️ 4. Topic Classification**
- **Method**: Keyword-based classification
- **Topics**: Technology, Mental Health, Education, Entertainment, Politics
- **Accuracy**: Manual validation performed

**📁 Files:** `notebooks/03_sentiment_topic_classification.ipynb`, `data/classified_reddit_data.csv`

### **📈 5. Visualization & Dashboard**
- **Power BI Dashboard**: Interactive visualizations
- **Public Deployment**: Published to Power BI Web Service
- **Features**: Real-time filtering, multiple visualizations

**📁 Files:** `dashboard/reddit_sentiment_dashboard.pbix`, `notebooks/05_powerbi_dashboard_setup.ipynb`

---

## 📊 **Key Results & Metrics**

| Metric | Value | Insight |
|--------|-------|---------|
| **Total Posts Analyzed** | 60 | Balanced across 3 subreddits |
| **Sentiment Distribution** | Positive: 42% | Mostly positive discussions |
| **Model Agreement Rate** | 85% | High consistency between VADER & TextBlob |
| **Most Common Topic** | Technology | Dominant in r/technology |
| **Dashboard Accessibility** | Public | No authentication required |
| **Data Reduction** | 25-40% | Through preprocessing |

---

## 🛠️ **Technology Stack**

| Component | Technology | Purpose |
|-----------|------------|---------|
| **Programming** | Python 3.9 | Main language |
| **Data Collection** | PRAW | Reddit API wrapper |
| **NLP Processing** | NLTK, TextBlob, VADER | Text analysis |
| **Data Manipulation** | Pandas, NumPy | Data processing |
| **Visualization** | Power BI, Matplotlib | Dashboard & charts |
| **Notebooks** | Jupyter, Google Colab | Development environment |
| **Version Control** | Git, GitHub | Code management |

---

## 📁 **File Details**

### **📓 Jupyter Notebooks:**
1. **`01_reddit_data_collection.ipynb`** - Complete Reddit API data collection
2. **`02_text_cleaning_preprocessing.ipynb`** - Full text preprocessing pipeline
3. **`03_sentiment_topic_classification.ipynb`** - Sentiment analysis + topic classification
4. **`04_data_visualization.ipynb`** - Data visualization code
5. **`05_powerbi_dashboard_setup.ipynb`** - Power BI dashboard creation

### **📄 Reports:**
1. **`PROJECT_SUMMARY_REPORT.pdf`** - Executive summary of the project
2. **`DETAILED_TECHNICAL_REPORT.pdf`** - Technical implementation details
3. **`METHODOLOGY_DETAILS.md`** - Step-by-step methodology
4. **`RESULTS_ANALYSIS.md`** - Detailed results interpretation

### **📊 Dashboard Files:**
1. **`reddit_sentiment_dashboard.pbix`** - Power BI dashboard file
2. **`dashboard_screenshot.png`** - Dashboard preview
3. **`powerbi_publication_proof.png`** - Publication confirmation

### **📈 Data Files:**
1. **`raw_reddit_data.csv`** - Original Reddit posts
2. **`preprocessed_reddit_data.csv`** - Cleaned text data
3. **`classified_reddit_data.csv`** - Final classified dataset

---

## 🚀 **Getting Started**

### **Prerequisites:**
- Python 3.9 or higher
- Reddit API credentials (for data collection)
- Power BI Desktop (optional, for dashboard editing)

### **Installation:**
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/reddit-sentiment-analysis-nlp-project.git
cd reddit-sentiment-analysis-nlp-project

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
