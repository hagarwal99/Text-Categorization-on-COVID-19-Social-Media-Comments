# Text Categorization on COVID-19 Social Media Comments


## Overview
The global impact of the COVID-19 pandemic has been profound, and social media platforms have emerged as pivotal channels for information and communication during this period. With millions of tweets posted daily, there is a growing necessity to analyze these tweets to gauge public sentiment regarding COVID-19. Our objective in this endeavor is to conduct Text analysis on COVID-19-related tweets utilizing the BERT (Bidirectional Encoder Representations from Transformers) classifier model.

## Data Set
The tweets have been pulled from Twitter and manual tagging has been done then. The names and usernames have been given codes to avoid any privacy concerns. You can find the dataset [here](https://www.kaggle.com/datasets/datatattle/covid-19-nlp-text-classification).<br><br>
**Columns:**
1) Location
2) Tweet At
3) Original Tweet
4) Label 


## Data Preprocessing
The data undergoes preprocessing using the Preprocessor class, which conducts several operations, including the removal of URLs, hashtags, mentions, and stop words. Additionally, the class handles text lemmatization.<br><be>


## Model
The BertClassifier class is designed to construct a model using the BERT model as its foundation, supplemented by additional fully connected layers for classification purposes. Within this class, the forward method accepts input text along with its attention mask and subsequently outputs the results of the classification task.


## Results :
Here are the results after **5** ephocs:<br>
Train accuracy: 96%<br>
Validation accuracy: 90%<br>
Test accuracy:  88%
<br>

## Inference Results
After training, the model can predict sentiment on new text data. Here are a few examples where the model made predictions:<br>

Text: this cant be worse. people are dying.
<br>Predicted Sentiment: Negative

Text: Good news is coming.
<br>Predicted Sentiment: Positive

Text: Another boring day in quarantine...
<br>Predicted Sentiment: Negative

Text: Second wave of #COVID19 in Delhi..back to more quarantine again...
<br>Predicted Sentiment: Neutral

Text: OK I'm angry now. I cannot believe the stupidity there is out there about #COVID19.
<br>Predicted Sentiment: Negative

Text: Thank GOD! Coronavirus: No deaths reported for 48 hours in Kerala.
<br>Predicted Sentiment: Positive

Text: I lost my cousine because of CORONAVIRUS last week. can't believe it...
<br>Predicted Sentiment: Negative

Text: Get the latest info and updates on #COVID19 on the Canada.ca
<br>Predicted Sentiment: Neutral

Text: I got vacinated today. Hope this #COVID19 ends soon.
<br>Predicted Sentiment: Positive

Text: supermarkets are running out of paper toilets. This is a shame for the gov!!!
<br>Predicted Sentiment: Negative
