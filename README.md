# 📰 Biased News Identification in Malayalam Media

This repository contains the research work and tools developed for identifying media bias in Malayalam news platforms using Natural Language Processing (NLP), data scraping, and analytical techniques.

## 📌 Project Overview

**Focus:** Identifying coverage, demographic, and gender bias in Malayalam digital news media using automated pipelines.

**Context:**  
- Malayalam is a low-resource language with limited computational tools.
- Digital news in India is dominated by Hindi and English, marginalizing regional narratives.

**News Sources:**
- **Malayala Manorama**
- **Kerala Kaumudi**
- **Mathrubhumi**

## 🧠 Objectives

- Collect and preprocess news data from selected Malayalam media platforms.
- Translate and standardize content for English-based NLP pipelines.
- Extract metadata using Named Entity Recognition and Classification.
- Quantitatively analyze and visualize bias in coverage.

## 🛠️ Tools and Technologies

- **Scraping:** `BeautifulSoup`, `Scrapy`, `Selenium`, `requests`, `xml.etree.ElementTree`
- **Translation:** `googletrans`, `IndicTrans2`
- **NLP & Tagging:** BERT-based NER, Zero-shot Classification
- **Analysis:** Entropy scoring, bias metrics on region, gender, and demography

## 📊 Data Collection

- Extracted from April 15–30, 2025
- Sources: RSS feeds, sitemaps, direct HTML parsing, and reverse-engineered dynamic requests
- Structured in CSV format with fields: `date`, `title (EN)`, `summary (EN)`, `source`, `url`, and generated tags

## 🔍 Bias Detection Methodology

- **Location Bias:** Entropy scores based on diversity of place mentions
- **Gender/Demographic Bias:** Ratio analysis for male/female representation and urban/rural disparity
- **Tagging Pipeline:** Named entities (persons, regions, organizations), event types, and keyword-based fallback tagging

## ⚠️ Challenges

- Semantic drift during Malayalam-to-English translation
- Cultural context loss in idiomatic expressions
- NER limitations on translated, context-poor data

## 📈 Key Findings

- ~62% of news focused on Trivandrum, Kochi, and Kozhikode
- Underreporting in Idukki, Kasaragod, and other rural areas
- Limited coverage of development and agriculture topics

## 🚀 Future Scope

- Implement emotion tagging and fine-grained sentiment classification
- Build interactive dashboards for bias and sentiment visualization
- Develop multilingual idiom corpora for improved NLP accuracy
- Collaborate with fact-checking networks for real-time alerts

## 🧾 Citation

If you use this research, please cite appropriately or mention this repository in your work.

## 📬 Contact

For questions or collaboration inquiries, feel free to open an issue or contact the author.
