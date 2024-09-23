# Kelompok 1 :
- Rayssa Ravelia  | 5025211219 |
- Dian Dabukke    | 5025211080 |

# CNN-Political-News-Scraper-and-Preprocessing

This project involves web scraping political news articles from CNN using 20 specific keywords. The scraped data is then preprocessed and explored through exploratory data analysis (EDA).

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Future Work](#future-work)

## Project Overview
The goal of this project is to scrape political news articles from CNN using 20 relevant keywords and preprocess the data for further analysis, such as sentiment analysis or named entity recognition (NER). The project includes web scraping using Selenium, basic exploratory data analysis (EDA), and data preprocessing to clean and prepare the dataset for downstream tasks.

### Keywords used for scraping:
- 'Government policy', 'Political corruption', 'Election results', 
  'Political debates', 'Legislative reforms', 'Foreign relations', 
  'Political parties', 'Campaign finance', 'Parliament decisions', 
  'Government scandals', 'Voter turnout', 'Lobbying efforts', 
  'Political protests', 'Human rights policies', 'Tax legislation', 
  'Trade agreements', 'National security policy', 'Immigration policy', 
  'Climate change legislation', 'Defense spending'

## Features
- **Web Scraping**: Scrapes political news articles from CNN using Selenium.
- **EDA (Exploratory Data Analysis)**: Analyzes the scraped data to understand distribution, keyword coverage, etc.
- **Data Preprocessing**: Cleans the raw data, handles missing values, formats dates, and prepares it for further analysis.

## Dataset
The dataset consists of 13,220 articles scraped from CNN, each associated with a keyword. The dataset contains the following features:
- **Keyword**: The search term used to find the article.
- **Title**: The headline of the news article.
- **Desc**: A short description or summary of the article.
- **Date**: The publication date of the article.
- **Link**: The URL to the article.

## Requirements
- Python 3.x
- Selenium
- Chrome WebDriver
- Pandas
- Numpy

Install the required libraries with the following command:
```bash
pip install -r requirements.txt
```

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/rayrednet/CNN-Political-News-Scraper-and-Preprocessing.git
   cd CNN-Political-News-Scraper-and-Preprocessing
   ```

2. Download and install Chrome WebDriver from [here](https://sites.google.com/a/chromium.org/chromedriver/) and place it in your working directory.

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. To start scraping, run the `scraper.py` script:
   ```bash
   python scraper.ipynb
   ```

2. The scraped data will be saved as a CSV file in the output folder.

3. To perform data preprocessing and EDA, run the `eda.ipynb` and 'preprocessing.ipynb' script

## Project Structure
```
├── data/
│   ├── scraped_cnn_news_100_pages_expanded.csv  # Scraped data
├── eda_preprocessing.ipynb                      # EDA and preprocessing script
├── scraper.ipynb                                # Web scraping script
├── README.md                                    # Project documentation
└── requirements.txt                             # Required Python packages
```

## Future Work
- **Sentiment Analysis**: Perform sentiment analysis on the dataset to categorize the sentiment of the articles.
- **Named Entity Recognition (NER)**: Extract key political entities from the news articles.
- **Topic Modeling**: Analyze the most discussed topics in political news using NLP techniques.
