---
layout: page
title: Projects
permalink: /projects/
description: A collection of my projects.
nav: true
nav_order: 2
---

Feel free to ping regarding any queries in these projects

### SEC Filings Analysis with LLM [May '24]
(Self Project) | [Project Link](https://github.com/srimanreddy4/Analysis-of-10k-fillings/tree/master)

- Extracted and cleaned 10,000 SEC filings from various companies, followed by data merging. Utilized Large Language Model (LLM) inference to generate comprehensive analyses and insights from the cleaned data
- Manually curated valuable insights from the LLM-generated analyses, and developed a web application that accepts a company ticker as input and generates data visualizations based on the corresponding SEC filings and insights.

### Food Delivery Database System [Feb '24 - Apr '24]
(Prof. Mayank Singh, IIT Gandhinagar) | [Project Link](https://github.com/Sparky1743/Food-Delivery-System-Website)

- Developed a comprehensive food delivery system for IIT Gandhinagar, involving stakeholder consultations, relational database design, frontend development using HTML, CSS, and Bootstrap, and backend implementation using Flask, Python, and SQL.
- The system includes features like SQL injection and XSS attack prevention, multi-user concurrent access, and Google authentication.

### Hugging Face Models Audit for Text Classification [Nov '23 - Feb '24]
(Prof. Mayank Singh, IIT Gandhinagar)

- Contributed as a co-author to an ARR 2024 submitted paper, exposing discrepancies between claimed and real-world performance, emphasizing need for transparent reporting in model efficacy.
- Conducted extensive in-domain and out-domain analysis, which included direct inference and finetuning on the top 100 downloaded models, utilizing three prominent datasets.
- Uncovered surprising findings that some lesser-known models with fewer downloads exhibited superior accuracy, emphasizing the existence of hidden gems in the field.

### Blithchron App, Blithchron, IIT Gandhinagar [June '23 - Nov '23]
[App Link](https://github.com/VivekRaj2005/blith-24-assets/raw/master/Blithchron24.apk)

- Developed and deployed the Flutter app for Gujarat's largest student-run cultural festival Blithchron.
- Skillfully integrated live quizzes, dynamic real-time location tracking, and crafted personalized user profiles featuring an intricate leaderboard system, all orchestrated with a robust Firebase backend.

### Drowsy Driving Detection using BCI Technology [Aug '23 - Dec '24]
(Prof. Krishna Miyapuram, IIT Gandhinagar) | [Project Link](https://github.com/srimanreddy4/EEG_drowsydriving)

- Implemented a robust machine learning model (SVM-RBF) trained on EEG data, achieving high accuracy for classifying attention states (focus, unfocus, drowsy); successfully deployed on an Arduino Nano using TensorFlow Lite and incorporating in a custom-designed 1-electrode EEG headset with 3D-printed components.

### Implementing Neural Causal model for Treatment effectiveness [Mar '24 - Apr '24]
(Prof. Anirban Dasgupta, IIT Gandhinagar) | [Project Link](https://drive.google.com/file/d/18YJwyBSgzyJWmnk7UhhH6mpoyWMusgZB/view?usp=sharing)

- Replicated the Dragonnet architecture from scratch for estimating the treatment effects from observational data using neural networks.
- Implemented Dragonnet and evaluate its performance on the IHDP and ACIC 2018 benchmark datasets for causal inference.

### Implementing GPT from Scratch [Mar '24]
(Self Project) | [Project Link](https://medium.com/@kondam.reddy/build-your-own-gpt-model-from-scratch-be73bd38bcb7)

- Implemented the paper ‘Attention is All You Need’ and built the transformer architecture from scratch to obtain a personalized language model trained on my own data.

### Reddit Sentiment Analysis and Visualization (NLP Project) [Sep '23]
(Prof. Mayank Singh, IIT Gandhinagar) | [Project Link](https://github.com/srimanreddy4/NLP-Assignment-1)

- Performed sentiment analysis on Reddit comments from a specific country's subreddit, using pre-trained models from Hugging Face and human annotations, and analyzed the results through exploratory data analysis and inter-annotator agreement.
- Created a word cloud visualization of the entire corpus, removing stop words and setting a minimum word length, to represent the prominent words and themes in the Reddit comments.

### N-gram Language Modeling on Reddit Data (NLP Project) [Sep '23]
(Prof. Mayank Singh, IIT Gandhinagar) | [Project Link](https://github.com/srimanreddy4/NLP_Assignment_2)

- Implemented unigram, bigram, trigram, and quadgram language models from scratch, without using any existing NLP library, and trained them on 80% of the Reddit data corpus, evaluating their performance on the remaining 20% using perplexity scores.
- Applied Laplace smoothing, as well as two other smoothing techniques (e.g., Additive, Good-Turing, or Kneser-Ney), to the language models, analyzing the impact of smoothing on perplexity scores and providing insights into the advantages and trade-offs of different smoothing methods.

### Pre-training and Fine-tuning Language Models (NLP Project) [Nov '23]
(Prof. Mayank Singh, IIT Gandhinagar) | [Project Link](https://github.com/srimanreddy4/NLP-Assignementt3)

- Pre-trained the BERT-base-uncased model on the WikiText-2 dataset for 5 epochs, computed perplexity scores on the test split, analyzed the score changes, and pushed the pre-trained model to the Hugging Face model repository.
- Fine-tuned the pre-trained model on two downstream tasks: sentiment classification (SST-2) and question answering (SQuAD), evaluated performance metrics specific to each task (e.g., accuracy, F1-score, ROUGE), compared model parameter counts before and after fine-tuning, and pushed the fine-tuned models to the Hugging Face repository.

### Facebook graph clustering based on density (Data Science Project) [Feb '24]
(Prof. Anirban Dasgupta, IIT Gandhinagar) | [Project Link](https://github.com/srimanreddy4/DataScience-HW)

- Implemented a greedy algorithm to extract the densest subgraph from Facebook's graph. Peeled the 5 densest graphs and analyzed their entropy. 

### Realtime Flutter Chat Application [Jan '23]
(Self Project) | [Project Link](https://github.com/srimanreddy4/Chat_application_flutter)

- Engineered a dynamic chat application with Google login, real-time messaging, and a robust Firebase backend and crafted personalized user profiles with an innovative UI design for the application.

### Air Quality forecasting using Language Models [Mar '23]
(Self Project) 

- Inspired by the research paper "Language Models are Zero-Shot Time Series Forecasters", downloaded the air quality dataset from the Central Pollution Control Board (CPCB) for the last two years.
- Set up the OllAMA language model locally, conducted time series forecasting experiments on the air quality data, and measured the results against a LSTM model as the baseline. 