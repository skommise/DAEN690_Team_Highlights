# DAEN690_Team_Highlights

Improved Methods for Measures of Profanity in Social Media Comments.

## Data
In the Data folder, resources from which the data is obtained:
  Twitter data: https://www.kaggle.com/ashwiniyer176/toxic-tweets-dataset (twitter_data.csv)
  Wikipedia data: https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/overview 
  combined_original_clean_data.xlsx: Cleaned, Wikipedia+twitter data
  tweet_translated.csv: Back translated data
  combined_original_bt_data.xlsx: Cleaned, Wikipedia + twitter_data + back_translated_data (Final dataset - Columns: text_data, profane_class: 1 if Profane, 0 if Not Profane)
  

## Scripts
This folder contains the scripts used throught the project:
  ### clean original data.ipynb 
    Datasets - twitter_data.csv, wikipedia.csv, combined_original_clean_data.xlsx
    This script is used to clean the original datasets using regular expressions and combine them. 
   
  ### Back translation model.ipynb
    Datasets - combined_original_clean_data.xlsx, tweet_translated.csv, combined_original_bt_data.xlsx
    This script is used to generate the synthetic data using back translation and combine the original datasets with back translated data. 
    
  ### Models:
  Final model contains the original and back translated data which has the text_data and the class label as the columns. The models are applied on the original data,        original+back_translated_data.
  ### Model 1 - Recurrent Neural Networks (LSTMs):
   ### LSTM_Original.ipynb
    LSTM model on the original dataset. Dataset used - combined_original_clean_data.xlsx. Accuracy- 92% , Precision- 91% , Recall- 92%
   ### LSTM_Original.ipynb
    LSTM model on the back translated dataset. Dataset used - tweet_translated.csv. Accuracy- 92% , Precision- 91% , Recall- 92%
   ### LSTM_Capstone-Orig+Back.ipynb
    LSTM model on the original+back translated dataset. Dataset used - combined_original_bt_data.xlsx. Accuracy- 94.3% , Precision- 94.2% , Recall- 94.5%
    
  ### Model 2- Feed Forward Neural Networks
   ### FFNN_model.ipynb
    FFNN model on the original dataset and the original+back translated dataset. Dataset used - combined_original_clean_data.xlsx, combined_original_bt_data.xlsx. 
    Orginal dataset - Accuracy- 72% , Precision- 73% , Recall- 72%
    Original+back_translated dataset - Accuracy- 76% , Precision- 76% , Recall- 76%

  ### Model 3 - Naive Bayes
   ### Naive_Bayes_Text Classification.ipynb
    NB model on the original dataset and the original+back translated dataset. Dataset used - combined_original_clean_data.xlsx, combined_original_bt_data.xlsx. 
    Orginal dataset - Accuracy- 90% , Precision- 92% , Recall- 87%
    Original+back_translated dataset - Accuracy- 92% , Precision- 94% , Recall- 89%
   
  ### Visualizations.ipynb
    Consists of the visualizations of the different n-grams in our datasets. 
 
 ### Team_Highlights_Showcase_Presentation_Slides.pptx 
  Contains final showcase presentation .pptx
  
 ### Team_Highlights_Final_Report.pdf
  Contains final project report
