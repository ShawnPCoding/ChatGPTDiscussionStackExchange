# ChatGPT Discussion Analysis on Data Science Stack Exchange

## Project Overview

This project analyzes discussions about ChatGPT on the Data Science Stack Exchange platform. By leveraging natural language processing (NLP), machine learning, and data visualization techniques, the study provides comprehensive insights into how the data science community perceives and interacts with ChatGPT technology.

## Table of Contents

- [Project Components](#project-components)
- [Dataset](#dataset)
- [Key Features](#key-features)
- [Analysis Methods](#analysis-methods)
- [Results](#results)
- [Ethical Considerations](#ethical-considerations)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Files and Directory Structure](#files-and-directory-structure)
- [Visualizations](#visualizations)

## Project Components

1. **Data Cleansing**: Processing and cleaning XML data from Stack Exchange
2. **Exploratory Data Analysis**: Statistical analysis of posts and comments
3. **Word and Topic Analysis**: Examining word frequencies and patterns
4. **Sentiment Analysis**: Analyzing emotional tone in discussions
5. **Correlation Analysis**: Exploring relationships between features
6. **Location Analysis**: Geographic distribution of discussions
7. **Thematic Analysis**: AI-powered categorization of discussion topics

## Dataset

The project uses Data Science Stack Exchange data in XML format, converted to CSV for analysis. Key datasets include:

- Posts
- Comments
- Users
- Tags
- Votes

## Key Features

- **Text Processing**: HTML removal, tokenization, lemmatization, stop word removal
- **Statistical Analysis**: Feature correlation, regression modeling
- **Sentiment Classification**: Positive, neutral, and negative sentiment identification
- **Topic Modeling**: Extraction of key themes and topics
- **Geospatial Visualization**: Geographic mapping of user discussions
- **Interactive Visualizations**: Dynamic charts and graphs

## Analysis Methods

- **NLP Processing Pipeline**: Cleaned and prepared text data using NLTK and regex
- **Sentiment Analysis**: Used VADER sentiment analyzer to classify text sentiment
- **Machine Learning**: Applied regression and scaling techniques for feature analysis
- **Word Clouds**: Generated visualizations of word frequencies by sentiment
- **Correlation Analysis**: Identified relationships between features like sentiment scores, code content, and engagement metrics
- **Thematic Analysis**: Used Ollama API (DeepSeek model) to categorize discussions into themes
- **Geospatial Analysis**: Mapped discussion distribution geographically

## Results

Key findings from the analysis:

- **Technical Focus**: 'Model' is the most frequent term in discussions, indicating a technical orientation
- **Sentiment Distribution**: Predominantly positive outlook in posts, with comments tending to be more neutral
- **Topic Categories**: Major discussion themes include technical implementation, ethical concerns, and practical applications
- **Feature Relationships**: Strong correlation between post scores and sentiment scores
- **Regional Variations**: Geographic patterns in user engagement and sentiment

## Ethical Considerations

The project addresses several ethical concerns:

1. **User Anonymity**: Ensuring no personally identifiable information is exposed
2. **Location Data Ethics**: Careful handling of user location information
3. **Bias in Data Representation**: Awareness of potential overrepresentation of certain regions or viewpoints
4. **Sentiment Misclassification**: Acknowledging limitations in algorithmic sentiment detection
5. **Thematic Analysis Integrity**: Avoiding oversimplification of complex user concerns
6. **Transparency**: Clear documentation of methods and tools used

## Installation and Setup

### Prerequisites

- Python 3.x
- Required Python packages (installable via pip):
  - pandas
  - numpy
  - nltk
  - scikit-learn
  - matplotlib
  - seaborn
  - folium
  - wordcloud
  - transformers

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/chatgpt-discussion-analysis.git
cd chatgpt-discussion-analysis

# Install dependencies
pip install -r requirements.txt

# For deep learning features (optional)
# Install Ollama for thematic analysis
curl -fsSL https://ollama.com/download/ollama-darwin-amd64 -o ollama
chmod +x ollama
sudo mv ollama /usr/local/bin/
ollama serve
ollama pull deepseek-r1:latest
```

## Usage

The analysis is structured as a Jupyter notebook:

```bash
# Open the notebook
jupyter notebook 1.8.ipynb
```

Alternatively, you can view the exported HTML report:

```bash
# Open the HTML report in a browser
open 1.8.html
```

## Files and Directory Structure

```
/
├── 1.8.ipynb                         # Main Jupyter notebook with analysis
├── 1.8.qmd                           # Quarto markdown version
├── merged_df.csv                     # Processed and merged dataset
├── datascience.stackexchange.com/    # Raw XML data folder
│   ├── Posts.xml
│   ├── Comments.xml
│   └── ...
├── csv_output/                       # Converted CSV data folder
│   ├── Posts.csv
│   ├── Comments.csv
│   └── ...
├── *.png                             # Static visualizations
└── *.html                            # Interactive visualizations
```

## Visualizations

The project includes various visualizations:

- Word clouds showing term frequency by sentiment
- Feature distribution plots
- Correlation heatmaps
- Sentiment comparison charts
- Thematic radial trees
- Geographic distribution maps
- Tag evolution charts

---

Developed by Hoang Son Pham (Student ID: 223240555) for SIT220 - Task 1.8HD
