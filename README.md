# Elon-Musk-Tweet-Generator   
In this fun project, I retrained a GPT2 language model with tweets from Elon Musk to create an Elon Musk Tweet Generator. Admittedly not a serious app, but a good exercise to take my LLM skills to the next level.  
  
## Notebook GPT2_ElonMuskPredictor.ipynb   
In this notebook, the data is first read in and subjected to preprocessing. In order to increase the data quality, only tweets of at least 7 words are left in the training data, mentions and URLs are removed and unnecessary punctuation and tick marks are eliminated.    
The cleaned data is tokenized and fed into the pre-trained distilgpt2 model.    
Finally the trained model is then tested and saved.    
  
## Notebook Musk_Tweets_API.ipynb   
This notebook contains an API created using FastAPI, which provides the created model for implementation and enables a call via Swagger UI.   
   
API Test:   
Click on the URL http://127.0.0.1:8000.   
The text {“message”: “This an Elon Musk Tweet Generator API test.”} appears.   
   
Swagger UI call:    
Append */docs* to the URL.  
A graphical user interface is displayed with which the application can be used directly, here by entering a prompt.   
(Click POST button and then Try it Out button.)   

## Elon Musk Tweets Data Source   
Source: https://www.kaggle.com/datasets/aryansingh0909/elon-musk-tweets-updated-daily?select=elonmusk.csv   
License: CC0: Public Domain    
