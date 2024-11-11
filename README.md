# COVID-19 Vaccine Sentiment Analysis on Twitter

This repository contains an implementation of the study **"Analyses of Public Attention and Sentiments towards Different COVID-19 Vaccines Using Data Mining Techniques"**. The study explores public sentiment regarding four COVID-19 vaccines (Covaxin, Moderna, Pfizer, and Sinopharm) using data mining techniques on Twitter data.

## Overview

This project aims to:
- Analyze public sentiment toward different COVID-19 vaccines.
- Track temporal trends in vaccine-related discussions.
- Map geographical sentiment distribution to identify regional differences in vaccine acceptance.

## Methodology

### 1. Data Collection
   - Tweets mentioning vaccine keywords (e.g., "Pfizer," "Moderna") were collected using Twitter API.
   - Filters were applied to exclude retweets, and only English-language tweets were included.

### 2. Data Preprocessing
   - Cleaned tweet text by removing URLs, punctuation, mentions, and stop words.
   - Converted text to lowercase and applied stemming/lemmatization to standardize words.

### 3. Sentiment Analysis
   - Utilized VADER sentiment analysis tool to categorize tweets as **Positive**, **Negative**, or **Neutral**.
   - Calculated compound sentiment scores to classify tweets (positive if score ≥ 0.05, negative if ≤ -0.05, and neutral otherwise).

### 4. Temporal and Geographical Analysis
   - **Temporal Analysis**: Tracked daily sentiment scores and volume of tweets over time to identify significant sentiment shifts.
   - **Geographical Analysis**: Mapped tweets based on user locations to observe sentiment distribution across different countries.

## Results Summary

- **Overall Sentiment**: Sentiments were largely neutral for all vaccines, with positive sentiments for Covaxin and Moderna at 28% and 37%.
- **Temporal Trends**: Pfizer and Sinopharm saw peaks in August 2021, Covaxin in July 2021.
- **Geographical Distribution**: India showed the highest positive sentiment for Covaxin, and the USA showed the highest positive sentiment for Moderna.

## Project Structure

- `data/`: Directory to store raw and processed tweet data.
- `src/`: Directory containing Python scripts for each part of the analysis.
- `notebooks/`: Jupyter Notebooks for exploratory data analysis and visualization.
- `results/`: Contains generated plots, figures, and summary tables.

## Getting Started

### Prerequisites
- Python 3.8 or above
- Twitter Developer Account for API access

### Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/yourusername/covid19-vaccine-sentiment-analysis.git
cd covid19-vaccine-sentiment-analysis
pip install -r requirements.txt


Usage
Configure Twitter API: Add your Twitter API credentials to config.py.
Run Data Collection: Execute the data_collection.py script to collect tweets based on vaccine-related keywords.
Run Sentiment Analysis: Use sentiment_analysis.py to perform sentiment classification on collected tweets.
Generate Visualizations: Execute visualization.py to create temporal and geographical sentiment visualizations.

Visualization Examples
Pie Chart: Overall sentiment distribution among vaccines.
Word Clouds: Most common words in positive, negative, and neutral tweets for each vaccine.
Temporal Plot: Daily trend of sentiment scores.
Geographical Heatmap: Regional sentiment distribution by country.
Contributing
Contributions are welcome! Please follow the standard GitHub fork-and-pull request workflow.


Contact
For further information, feel free to contact the authors or submit an issue on GitHub.

This `README.md` should serve as a comprehensive introduction to the project, guiding users through setup, usage, and key project features. Let me know if you need additional sections or modifications!
