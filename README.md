# LinkedIn Top Posts --- End-to-End Classification, EDA and Regression Analysis.
## Project Overview:
LinkedIn offers Impressions & Engagements data for top 50 posts. The aim of this project is to scrape those posts, assigning attributions, classifying them into categories, performing full Exploratory Data Analysis with Data Visualization and applying regression analysis to find guiding weights.

## Data License and Attribution:
Data inside the 'Posts' folder is my personal top 50 posts provided by LinkedIn and available for public use.

## Files & Folders:
1. requirements.txt:
    * Project Dependencies.
1. Posts (Folder):
    * A directory containing scraped posts stored in .txt files.
    * Each .txt file has the following format: post_id-attachment_type.txt
1. 01- Data Extraction & Posts Classification.ipynb:
    * Extracting data from 'Posts' directory.
    * Classifying posts into categories using MoritzLaurer/mDeBERTa-v3-base-mnli-xnli.
1. 02- EDA.ipynb:
    * Exploratory Data Analysis & Data Visualization.
1. 03- ML Model & Weights.ipynb:
    * Linear Regression & Hyper-Parameters Tuning with ElasticNet using scikit-learn with Cross Validation.


## Process:
1. Top posts analysis download from LinkedIn .
1. Manual posts scraping & attribution.
1. Posts content exctraction and DataFrame structuring.
1. Post classification.
1. Feature Engineering.
1. Exploratory Data Analysis.
1. Machine Learning Modeling, Cross Validation and Hyper-Parameters tuning.
1. Weights ectraction and interpretation.


## Libraries Used:
1.matplotlib=3.10.8
1. numpy=2.2.5
1. pandas=2.3.3
1. scikit-learn=1.7.2
1. seaborn=0.13.2
1. transformers=5.2.0


## Conclusion:
1. Impressions:
   * Day of Week: Posting on Sunday increases impressions by 4.77% compared to other days of the week.
   * Post Style: Professional post style increases impressions by 1.64% compared to other styles.
  
2. Engagements:
   * Day of Week: Posting on Sunday increases engagements by 0.93% compared to other days of the week.
   * Attachments: Attaching a single Image increases engagements by 0.85% compared to videos, multiple images or no attachments.
   * Post Category: Educational Content increases engagements by 0.77% compared to other categories.
  
## Limitations:
* **Dataset Size:** The analysis and machine learning models are based on a limited sample size (top 50 posts). Although ElasticNet with Cross-Validation was utilized to mitigate overfitting, the predictions and feature weights should be treated as directional insights rather than absolute, generalizable rules.
* **Context Specificity:** The findings strictly reflect the performance of my personal LinkedIn content and the engagement behavior of my specific network. Engagement patterns, optimal posting days, and content preferences may vary significantly for other profiles, industries, or target audiences.
