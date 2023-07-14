# NLP Sentiment Analysis on Hotel Reviews
This repository contains a project on sentiment analysis using Natural Language Processing (NLP) techniques to analyze hotel reviews and predict their sentiment. The project focuses on a dataset of hotel reviews obtained from the Hugging Face platform's Tripadvisor Hotel Reviews dataset.
PS. In the presentation, I chose Marriot International Hotel as my stakeholder to present this project too, but in reality, there are many reviews from different hotel chains. 

![black-wordcloud](https://github.com/wasih790/Project_4_Hotel_Sentiment_Analysis/assets/120667351/de745a64-b5a9-444d-abed-a9308de97af0)


## Dataset
The dataset used for this project can be found on the Hugging Face platform at the following link: https://huggingface.co/datasets/argilla/tripadvisor-hotel-reviews/viewer/argilla--tripadvisor-hotel-reviews/train?row=0, It consists of 20,491 rows, containing reviews and ratings ranging from 1 to 5. The dataset was preprocessed by adding a new column called 'Label' to predict whether a review is negative or positive. Reviews with ratings 4 and above are considered positive, while ratings 3 and below are considered negative.

## Objective
The objective of this project is to perform sentiment analysis on the hotel reviews dataset and develop predictive models to classify reviews as either positive or negative. Additionally, topic segmentation was performed to identify the main topics discussed in the reviews.

![Screenshot 2023-07-11 at 8 57 35 PM](https://github.com/wasih790/Project_4_Hotel_Sentiment_Analysis/assets/120667351/279a6553-9d7f-468e-99f8-679fd19be2f2)


## Topic Segmentation
Topic segmentation was conducted to categorize the reviews into different topics based on their content. Five topics were identified during the analysis:

1. City Experience
2. Value & Comfort
3. Guest Interaction & Experience
4. Restaurant Experience
5. Resort

![Screenshot 2023-07-13 at 3 41 26 PM](https://github.com/wasih790/Project_4_Hotel_Sentiment_Analysis/assets/120667351/6a5eb895-5d4b-4e13-83e7-ef0c714faebd)


An interesting finding from the analysis is that a significant number of negative reviews were associated with the "Guest Interaction & Experience" topic. To address this, a recommendation was made to hotels to enhance guest satisfaction by providing better customer service and training staff on customer service etiquette.

Furthermore, positive reviews were found to be strongly linked to the resort where guests stayed, particularly in the case of beach resorts. To maintain positive reviews, it was suggested that hotels should invest in improving the beauty and greenery of their locations by hiring gardeners and landscapers. The significance of the location, especially for resorts situated near the beach, was emphasized.

## Models and Results
Two different models were developed to predict the sentiment labels of the hotel reviews.

1. Complement Naive Bayes Model:

- Model Type: Complement Naive Bayes
- Features: Words from the reviews
- Accuracy: 80%
- AUC Score: 89%

2. Logistic Regression Model with Sentiment Intensity Analyzer:
- Model Type: Logistic Regression
- Features: Text from the reviews and sentiment intensity analyzer scores
- Accuracy: 89%
- AUC Score: 93%

The second model, which incorporated sentiment intensity analyzer scores along with the review text, achieved higher accuracy and AUC scores compared to the first model. This suggests that considering the sentiment intensity of the reviews improves the predictive performance.

![Screenshot 2023-07-12 at 7 03 30 PM](https://github.com/wasih790/Project_4_Hotel_Sentiment_Analysis/assets/120667351/0ea583a4-e07c-40a5-83fd-932d57b057c4)


# Code and Implementation
The code for this project can be found in the Sentiment Analysis folder. It includes data preprocessing steps, exploratory data analysis, topic segmentation, model training, and evaluation.

Dependencies
The following dependencies are required to run the code:

- Python 3.7 or above
- Natural Language Toolkit (NLTK)
- Scikit-learn
- Pandas
- Matplotlib
- Seaborn
- Plotly
Please ensure that these dependencies are installed before running the code.

# Conclusion
This project demonstrates the application of NLP techniques for sentiment analysis on hotel reviews. By analyzing the dataset, identifying topics, and developing predictive models, valuable insights were gained regarding guest experiences and resort locations.

The findings suggest that hotels should focus on improving guest satisfaction by training staff on customer service etiquette. Additionally, investments in enhancing the beauty and greenery of resort locations, especially those situated near beaches, can help maintain positive reviews.

By leveraging the power of NLP and sentiment analysis, hotel management can make informed decisions to enhance customer experiences and drive positive sentiment in reviews, ultimately improving overall customer satisfaction and reputation.

Feel free to explore the code, dataset, and results in this repository to gain a deeper understanding of the project.
