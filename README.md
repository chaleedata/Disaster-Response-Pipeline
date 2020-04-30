# Disaster-Response-Pipeline

## Description:
In this app, a machine learning pipeline is created to classify the emergency messages sent by users to appropriate categories. The data for training is obtained from Figure Eight Disaster Response Data. The data thus obtained is cleaned and transformed to the necessary form using the ETL pipelines and other Data Engineering techniques. Then a front-end is created using the HTML and deployed using the python FLASK library. Visit the below link for more information on Flask.

This project is divided in the following key sections:

1. Processing data, building an ETL pipeline to extract data from source, clean the data and save them in a SQLite DB
2. Build a machine learning pipeline to train the which can classify text message in various categories
3. Run a web app which can show model results in real time

## Getting Started
### Dependencies
- Python 3.5+
- Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
- Natural Language Process Libraries: NLTK
- SQLlite Database Libraqries: SQLalchemy
- Model Loading and Saving Library: Pickle
- Web App and Data Visualization: Flask, Plotly

To clone the git repository:
<pre><b> git@github.com:chaleedata/Disaster-Response-Pipeline.git</pre>

### Executing Program:
1. You can run the following commands in the project's directory to set up the database, train model and save the model.

  - To run ETL pipeline to clean data and store the processed data in the database python python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db
  - To run the ML pipeline that loads data from DB, trains classifier and saves the classifier as a pickle file python python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl

2. Run the following command in the app's directory to run your web app. python run.py

3. Go to http://0.0.0.0:3001/

### Additional Material
In the data and models folder you can find two jupyter notebook that will help you understand how the model works step by step:

  1. ETL Preparation Notebook: learn everything about the implemented ETL pipeline
  2. ML Pipeline Preparation Notebook: look at the Machine Learning Pipeline developed with NLTK and Scikit-Learn

You can use ML Pipeline Preparation Notebook to re-train the model or tune it through a dedicated Grid Search section. In this case, it is warmly recommended to use a Linux machine to run Grid Search, especially if you are going to try a large combination of parameters. Using a standard desktop/laptop (4 CPUs, RAM 8Gb or above) it may take several hours to complete.

### Authors
[Chalee](https://github.com/chaleedata)

### Licence 
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Acknowledgements
- [Udacity](https://www.udacity.com/) for providing such a complete Data Science Nanodegree Program
- [Figure Eight](https://appen.com/) for providing messages dataset to train my model
