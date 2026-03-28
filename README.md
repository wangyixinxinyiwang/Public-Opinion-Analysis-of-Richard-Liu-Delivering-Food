[README.md](https://github.com/user-attachments/files/26322814/README.md)
# 🛒 Public Sentiment Analysis: Richard Liu Delivery Event (Cross-Platform Study)

> **Project Type:** Data Analytics, Social Media Mining & Natural Language Processing (NLP)  
> **Tech Stack:** Web Scraper, Python (Pandas, Matplotlib, WordCloud), Hugging Face (DistilBERT), Jupyter Notebook

---

## 📖 1. Project Overview
In the era of fragmented information, identifying genuine public sentiment while stripping away emotional bias is a core challenge. This project takes the social hot topic of "Richard Liu (CEO of JD.com) personally delivering takeout" as a case study. 

The primary objective is to collect, clean, and analyze user comments across two distinct Chinese social media ecosystems: **Douyin** (TikTok China) and **Xiaohongshu** (RED). By leveraging AI-driven sentiment analysis, this project explores how the exact same event triggers completely different emotional responses and community discussions based on platform culture.

---

## 🗂️ 2. Repository Structure
The project is organized as follows to ensure reproducibility and clear data flows:

    ├── data/
    │   ├── douyin2.xlsx                                      # Raw scraped comments from Douyin
    │   └── xiaohongshu2.xlsx                                 # Raw scraped comments from Xiaohongshu
    ├── notebooks/
    │   ├── 刘强东送外卖舆情分析_抖音.ipynb                   # Source code for Douyin analysis
    │   └── 刘强东送外卖舆情分析_小红书.ipynb                 # Source code for Xiaohongshu analysis
    ├── images/
    │   ├── Count of Sentiment Categories - Douyin.png
    │   ├── Count of Sentiment Categories - Xiaohongshu.png
    │   ├── Distribution of Sentiment Scores - Douyin.png
    │   ├── Distribution of Sentiment Scores - Xiaohongshu.png
    │   ├── Proportion of Sentiment Categories - Douyin.png
    │   ├── Proportion of Sentiment Categories - Xiaohongshu.png
    │   ├── Word Cloud of Adjectives in Comments - Douyin.png
    │   └── Word Cloud of Adjectives in Comments -Xiaohongshu.png
    └── README.md

---

## ⚙️ 3. Analytical Pipeline
1. **Data Collection:** Utilized Web Scraper to extract first-hand user comments, resulting in the foundational datasets (`douyin2.xlsx` and `xiaohongshu2.xlsx`).
2. **Data Preprocessing:** Deployed `pandas` to handle missing values and utilized Regular Expressions (`re`) to strip out emojis, special characters, and non-textual noise.
3. **AI Sentiment Analysis:** Implemented Hugging Face's open-source multi-lingual LLM (`distilbert-base-multilingual-cased`) to automatically classify thousands of comments into **Positive**, **Neutral**, or **Negative** sentiments.
4. **Data Visualization:** Used `matplotlib` and `WordCloud` to generate comparative charts and extract high-frequency adjectives, mapping out the emotional landscape of each platform.

---

## 📊 4. Cross-Platform Visualizations

To intuitively illustrate the divergence in audience reception, the analysis results from Douyin (Left) and Xiaohongshu (Right) are presented side-by-side below.

### 📌 4.1 Proportion of Sentiment Categories
*Observation: Douyin comments are dominated by strong negative emotions, whereas Xiaohongshu exhibits an overwhelmingly neutral, "bystander" attribute.*

| 🎵 Douyin | 📕 Xiaohongshu |
| :---: | :---: |
| ![Proportion Douyin](images/Proportion%20of%20Sentiment%20Categories%20-%20Douyin.png) | ![Proportion Xiaohongshu](images/Proportion%20of%20Sentiment%20Categories%20-%20Xiaohongshu.png) |

### 📌 4.2 Counts & Distribution of Sentiment Scores
*Observation: Cross-validation through bar charts and histograms further confirms that Douyin's emotional inclination is significantly "left-skewed" (Negative), while Xiaohongshu is "centered" (Neutral).*

| 🎵 Douyin | 📕 Xiaohongshu |
| :---: | :---: |
| ![Count Douyin](images/Count%20of%20Sentiment%20Categories%20-%20Douyin.png) | ![Count Xiaohongshu](images/Count%20of%20Sentiment%20Categories%20-%20Xiaohongshu.png) |
| ![Score Douyin](images/Distribution%20of%20Sentiment%20Scores%20-%20Douyin.png) | ![Score Xiaohongshu](images/Distribution%20of%20Sentiment%20Scores%20-%20Xiaohongshu.png) |

### 📌 4.3 Word Cloud of Adjectives
*Observation: Word clouds reveal the specific triggers behind the emotions—what exactly are netizens discussing?*

| 🎵 Douyin | 📕 Xiaohongshu |
| :---: | :---: |
| ![Word Cloud Douyin](images/Word%20Cloud%20of%20Adjectives%20in%20Comments%20-%20Douyin.png) | ![Word Cloud Xiaohongshu](images/Word%20Cloud%20of%20Adjectives%20in%20Comments%20-Xiaohongshu.png) |

---

## 💡 5. Conclusion & Reflections

### 🔍 Cross-Platform Insights
Through rigorous data comparison, this project yielded the following core conclusions:
1. **Douyin (Highly Critical):** The public opinion environment is highly polarized and critical. Users tend to view this event through a macro-socioeconomic lens, frequently associating high-frequency words with negative sentiments. They view the event as a deliberate "PR stunt," exhibiting strong defensiveness against corporate actions.
2. **Xiaohongshu (Lifestyle-Oriented):** The community atmosphere is mild and decentralized. Over half of the users maintain a neutral stance. The focus of the discussion shifts from "macro-social issues" down to specific "lifestyle details" (e.g., outfits, personal takeout experiences), showing typical "bystander" behavior.
3. **Commercial Implications:** Modern corporate crisis management or marketing campaigns cannot adopt a "one-size-fits-all" strategy. Content delivery must be highly customized based on the unique cultural DNA of each platform.

### ⚖️ Ethical Considerations
* **Technical Limitations:** Although AI NLP models significantly improve analysis efficiency, they still face risks of misjudgment when dealing with complex internet slang, sarcasm, and rhetorical nuances.
* **The Necessity of Human Insight:** Data only provides phenomena; it does not provide explanations. In this project, sociological theories and communication perspectives gave the raw data its true value. Technology should serve professional judgment, not replace humanistic gatekeeping.

## 🚀 6. Future Work
To further deepen this research and expand its analytical dimensions, the following areas can be explored in future iterations:

* **Expanded Multi-Platform Analysis:** Extend the data collection to include other major social networks such as **Weibo** (news and text-centric) and **Bilibili** (long-form video, younger demographic) to construct a more holistic map of Chinese public opinion.
* **Geospatial Sentiment Analysis (IP Location):** Leverage the IP address location tags associated with user comments to conduct regional analysis. This will help determine if sentiment correlates with geographic locations, mapping out how coastal vs. inland provinces, or tier-1 vs. tier-3 cities, react differently to corporate events.
