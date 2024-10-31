# Greek News Sites Web Scraping and Sentiment Analysis Project

## Project Overview

This project focuses on web scraping articles from various Greek news websites, with the goal of gathering a substantial dataset of news articles. The collected data will then be processed using Natural Language Processing (NLP) techniques to perform sentiment analysis and identify patterns in language use, particularly with respect to polarized language or divisive rhetoric. This repository will include the scripts for scraping, data storage, and initial analysis.

## Objectives

1. **Data Collection**: Extract a significant number of articles from each target news website.
2. **Data Fields**: For each article, the following details will be collected:
   - Website URL
   - Publication Date
   - Author's Name
   - Title
   - Full Article Content
   - *(Optional) Extracted Words Count per Article (for extra measurments)*
3. **NLP and Sentiment Analysis**: Process and analyze collected articles to uncover any tendencies toward polarized or divisive language.

## Data Structure and Storage

To streamline the data storage and analysis process, all collected data will be saved in CSV, json or text files. Each file will have the following column names, which will directly correspond to the column names in a PostgreSQL database for easy import:
- **Files Column Names**: `site_url`, `issue_date`, `author_name`, `article_title`, `article_content`

## Database Setup

The project will start by setting up a PostgreSQL database with tables reflecting the data columns above. After database setup, targeted scraping scripts will extract the specific fields listed from the HTML content of each article, ensuring uniform data structure and quality.

## Getting Started

This repository will provide:
- **Scraping Scripts**: Python scripts designed to navigate the structure of each site and collect only the specified information.
- **Database Configuration**: SQL scripts or instructions for setting up the PostgreSQL database.
- **Sentiment Analysis & NLP Scripts**: Extra Python scripts designed to apply Natural Language Processing techniques on the extracted information.

As the project progresses, updates may be made to include additional fields (such as word count) and to improve the sentiment analysis capabilities, and more advanced metrics.

## Future Steps

Once data collection is complete, the next steps will involve detailed NLP and sentiment analysis. Results will help identify patterns in media language use and contribute insights into the presence of polarized or divisive rhetoric in Greek news sources.
