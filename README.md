# Public-Opinion-Analysis-of-Richard-Liu-Delivering-Food
This project provides a comprehensive sentiment analysis of public comments concerning Richard Liu (Liu Qiangdong) acting as a food delivery driver, includING: Data Preparation, Sentiment Scoring, Sentiment Categorization, Visualizations.
# Public Sentiment Analysis: Liu Qiangdong's Delivery Event (Cross-Platform Study)

> **Project Type:** Data Analytics, Social Media Mining & Sentiment Analysis  
> **Role:** Data Analyst & Visualizer  
> **Tech Stack:** Web Scraper, Python (Pandas, Matplotlib), AI/NLP (Hugging Face DistilBERT), Google Colab  

[![Open In Colab - Douyin](https://colab.research.google.com/assets/colab-badge.svg)](替换为你的抖音Colab链接) 
[![Open In Colab - Xiaohongshu](https://colab.research.google.com/assets/colab-badge.svg)](替换为你的小红书Colab链接)

## 1. Project Overview (项目概述)
In the era of fragmented information, identifying genuine public sentiment while stripping away emotional bias is a core challenge. This project takes the social hot topic of "Liu Qiangdong delivering takeout" as a case study. By tracking public emotion evolution across different social media ecosystems (**Douyin** vs. **Xiaohongshu**), the project aims to distill key societal issues and enhance data-driven decision-making skills.

## 2. Data Sources & Methodology (数据与方法论)
We constructed an automated pipeline combining traditional data cleaning with advanced AI inference:
* **Data Collection:** Utilized Web Scraper to extract first-hand user comments from Douyin and Xiaohongshu (exported as `.xlsx` datasets).
* **Data Preprocessing:** Used Python's `pandas` and `re` modules to clean the text, removing null values and non-textual noise.
* **AI Sentiment Analysis:** Deployed a lightweight multi-lingual NLP model (`distilbert-base-multilingual`) via Hugging Face to automatically classify texts into Positive, Neutral, and Negative sentiments.
* **Data Visualization:** Used `matplotlib` to convert textual data into intuitive charts, enabling cross-platform comparative analysis.

## 3. Visualizations & Outcomes (成果展示)
*(Student Note: Insert your Matplotlib chart screenshots here. You can show a comparison between the two platforms.)*

### 📊 Douyin Sentiment Distribution
![Douyin Chart](替换为你的抖音图表图片名称.png)

### 📊 Xiaohongshu Sentiment Distribution
![Xiaohongshu Chart](替换为你的小红书图表图片名称.png)

## 4. Cross-Platform Insights (平台差异洞察)
*(Student Note: Write 1-2 sentences comparing the two platforms. E.g., Did Douyin have more negative comments regarding the "PR stunt"? Was Xiaohongshu more focused on the work environment?)*
* **Douyin:** [Add observation here]
* **Xiaohongshu:** [Add observation here]

## 5. Reflection & Ethical Considerations (反思与伦理)
* **Technical Limitations:** While AI greatly enhances data processing efficiency, it occasionally misjudges complex contexts and sarcasm. The algorithms may also inadvertently amplify algorithm bias if the training data is skewed.
* **Interdisciplinary Synergy:** Technology is not a panacea. True insight comes from the synergy of **"Multi-platform Data + AI Assistance + Human Deep Analysis"**. By using communication theories as a framework and data science as a tool, we achieve a dynamic balance between rational algorithms and humanistic perspectives.
