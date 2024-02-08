Background

Axon is the leading provider of public safety technology solutions, which includes body cameras and digital evidence management systems. The company is deeply invested in customer experience and uses Net Promoter Score (NPS) as a key metric to measure customer satisfaction and to incentivize all Axon employees to prioritize customer needs. Axon runs an NPS based customer survey throughout the year, gathering thousands of responses annually to continually measure and shape the customer experience. 
Axon uses NPS as a key metric to measure customer satisfaction and proactively address any potential issues. They classify survey responses into 6 categories and prioritize areas of improvement based on NPS scores to enhance the customer experience.

Project Proposal

Using machine learning to categorize customer feedback into 6 categories: “Product”, “Cost”, “Customer Service”, “Training”, “Sales”, and “Others”. This will help Axon proactively identify problems and streamline the process. By reducing the manual effort required for categorization, machine learning models will provide accurate results, ultimately leading to better customer satisfaction and an improved NPS score.

Installation Instructions

To use the code in your Python environment, you will need to install the following libraries:

Pandas: pip install pandas (Version: 1.4.4)
NumPy: pip install numpy (Version: 1.23.5)
Seaborn: pip install seaborn (Version: 0.12.2)
Matplotlib: pip install matplotlib (Version: 3.6.2)
Plotly: pip install plotly (Version: 5.9.0)
ipywidgets: pip install ipywidgets (Version: 7.6.5)
Scikit-learn: pip install scikit-learn (Version: 1.1.2)
imbalanced-learn (for SMOTE): pip install imbalanced-learn (Version: 0.10.1)
statsmodels: pip install statsmodels (Version: 0.13.5)
spaCy: pip install spacy (Version: 3.3.1)
gensim: pip install gensim (Version: 3.4.0)


en_core_web_lg, a pre-trained English language model from the Spacy library, which is designed for processing English language text. It is a large language model that has been trained on a diverse range of text, including news articles, web pages, and scientific publications, to perform various NLP tasks such as part-of-speech tagging, named entity recognition, and dependency parsing.
The word2vec-google-news-300 is a pre-trained model using the word2vec algorithm on a large corpus of Google News articles, generating 300-dimensional word vectors for a vocabulary of around 3 million words. As the model was trained on a large corpus of text from Google News articles—covering a broad range of topics, including business and finance—the model is likely to have seen a significant number of articles about Axon and its products and may have learned useful embeddings for these terms.

Usage Guide

The folder contains 2 jupyter notebook, generate_model.ipynb , generate_output.ipynb, 
Takes input from NPS Data for ASU Team.csv

1. generate_model.ipynb, needs to run a csv file in Axon format (NPS Data for ASU Team.csv) which consists of classified records. The model trains on the following data file. Tunes hyperparameters and asks for probability threshold for all the six models for each category then saves the model parameters in a dictionary format (model) as a pickle file. The pickle file is saved in the main directory, along with a backup folder is created with the name model_datetime which also contains the model. This file also saves the spacy model (spacy_model_updated_v2), and the word vector file (word2vec-google-news-300) in the main directory.

2. generate_output.ipynb, once the model has been generated this file runs and takes the pickle file, the space model, and google vectors as the inputs along with the csv file by the name (NPS Data for ASU Team Output.csv) and generates the output with all the categorized records and saves them as (Categorized_Data_datetime.csv)

Contact Information

Contact information for the project maintainers or contributors in case users have questions or encounter issues.
Amit Manocha | amit.manocha1995@gmail.com | +1 (602) 516-5446
Siri Kademani   |
Helen Kim         |
Supratim Roy    |
