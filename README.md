# Analysis of Public Sentiment and Discussion Topics on the Israeli-Palestinian Conflict

This project analyzes public sentiment and discussion topics on the Israeli-Palestinian conflict using YouTube comments from major news channels. By leveraging Natural Language Processing (NLP) models, including BERT for sentiment analysis and BERTopic for topic modeling, the study examines how digital discourse evolves over time and across different news networks.

# Files
- Dataset  = Folder containing the dataset used for fine-tuning BERT, the 6 datasets of the analyzed videos, and the 6 datasets of the videos with their respective predictions.
- img = folder containing the plots
- quarto_paper = folder containing the quarto file to run the paper: Braga_Christian_paper.qmd, and the pdf of the paper: Braga_Christian_paper.pdf
- Research_Design_CSS_Project_Christian_Braga.pdf: research desing of the project
- dataset_creation.ipynb = code used to build the datasets
- BERT_model.ipynb = code used to create the BERT model used in the sentiment analysis
- BERT-topic_model.ipynb = code used to create the BERT-topic model used in the topic modelling analysis
- requirements.txt = dependencies for the creation of the virtual env

# Installation / Run
The models have been developed on google collab using the T4 GPU, to run the files of the models click on the file's names (BERT_model.ipynb and BERT-topic_model.ipynb) and click on the button : ![Screenshot 2025-03-18 at 14 37 07](https://github.com/user-attachments/assets/c9555b95-a463-42f8-bf66-e702d92e5209) to open a Google Collab notebook and run all the cells.

To correctly run the QMD file, ensure that you have Python installed and that the Quarto extension is set up in your IDE. Follow these steps to set up the environment and execute the project:
- Download or clone this repository to your local machine
- Inside the cloned repository, create a virtual environment to manage dependencies
- Once the virtual environment is activated, install the necessary dependencies from the requirements.txt file: pip install -r requirements.txt
- Run / render the .qmd file of the project

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
