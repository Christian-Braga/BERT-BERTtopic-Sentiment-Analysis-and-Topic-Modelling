# Analysis of Public Sentiment and Discussion Topics on the Israeli-Palestinian Conflict

This project analyzes public sentiment and discussion topics on the Israeli-Palestinian conflict using YouTube comments from major news channels. By leveraging Natural Language Processing (NLP) models, including BERT for sentiment analysis and BERTopic for topic modeling, the study examines how digital discourse evolves over time and across different news networks.

# Project Structure

- **`Dataset/`**  
  Contains all datasets used in the project:
  - Dataset for fine-tuning the BERT model.
  - Six datasets corresponding to the analyzed videos.
  - Six datasets including the videos with their respective predictions.

- **`img/`**  
  Folder containing all the generated plots and visualizations.

- **`quarto_paper/`**  
  Contains the source and output of the project paper:
  - `Braga_Christian_paper.qmd`: Quarto source file to compile the paper.
  - `Braga_Christian_paper.pdf`: Final PDF version of the paper.

- **`Research_Design_CSS_Project_Christian_Braga.pdf`**  
  Research design document outlining the objectives, methodology, and structure of the project.

- **`dataset_creation.ipynb`**  
  Jupyter notebook used for preprocessing and constructing the datasets.

- **`BERT_model.ipynb`**  
  Notebook for training and evaluating the BERT model used in the sentiment analysis.

- **`BERT-topic_model.ipynb`**  
  Notebook implementing the BERT-based topic modeling approach.

- **`requirements.txt`**  
  List of dependencies required to set up the virtual environment for the project.

# Installation / Run
The models have been developed on google collab using the T4 GPU, to run the files of the models click on the file's names (BERT_model.ipynb and BERT-topic_model.ipynb) and click on the button : ![Screenshot 2025-03-18 at 14 37 07](https://github.com/user-attachments/assets/c9555b95-a463-42f8-bf66-e702d92e5209) to open a Google Collab notebook and run all the cells.


## Prerequisites
- Python installed on your system
- Quarto extension properly set up in your IDE (VS Code or RStudio)

## Getting Started

### Clone the Repository
```bash
git clone https://github.com/Christian-Braga/BERT-BERTtopic-Sentiment-Analysis-and-Topic-Modelling.git
cd BERT-BERTtopic-Sentiment-Analysis-and-Topic-Modellin
```

### Environment Setup
Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate # On Windows use: .venv\Scripts\activate
```

### Install Dependencies
Install all required packages:
```bash
pip install -r requirements.txt
```

### Render the Paper
Generate the final document:
```bash
quarto render quarto_paper/Braga_Christian_paper.qmd
```

> 💡 **Note:** Make sure Quarto is installed on your system. Download it from [https://quarto.org](https://quarto.org) and verify the installation with `quarto check`.


# Project Overview

This study investigates public sentiment on the Israeli-Palestinian conflict by analyzing comments from YouTube videos published by:
Al Jazeera English
CNN
Sky News
The project explores sentiment trends over time, comparing October 2023 (after a pivotal event) with data from 2024. Additionally, it examines the impact of different news channels on public perception.

# Dataset Collection

The dataset consists of YouTube comments extracted from six videos published by the selected news channels. The YouTube API was used to retrieve comments, filtering them based on language and relevance.

# Sentiment Analysis

The fine-tuned BERT model was trained on 1,486 manually labeled comments to classify sentiment into three categories:
Pro-Israel
Pro-Palestine
Neutral
The model achieved an accuracy of 76%, despite challenges such as irony, sarcasm, and implicit bias.

# Topic Modeling

Using BERTopic, the project identified key discussion topics from the comments. Some significant findings:
Pro-Israel comments often discussed hostages, security concerns, and media bias.
Pro-Palestine comments included themes of humanitarian crises, historical comparisons, and religious narratives.
Neutral comments focused on media credibility, propaganda, and the geopolitical landsca

# Results

📊 Findings from the analysis include:

A shift from neutral to more polarized opinions over time.
Al Jazeera had the highest proportion of Pro-Israel comments.
CNN had the highest proportion of Pro-Palestine comments.
Sky News remained relatively balanced, with fewer biases discussed.

Sentiment Over Time
The percentage of neutral comments decreased from 43.5% in 2023 to 37.2% in 2024.
Support for Palestine increased by nearly 6%, while Pro-Israel comments remained stable.

Perception of Media Bias
Many comments questioned the credibility of news sources, particularly Al Jazeera and CNN.
Some users accused channels of biased reporting, reflecting a critical engagement with media narratives.
