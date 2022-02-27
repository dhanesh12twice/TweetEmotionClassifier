#Tweet Emotion Classifier/Recogniser Model

<br />
<br />

###Description:
       This project is all about recognising what emotion is inscribed on the tweet. This is a supervised classification problem of classes- joy,sadness,surprise,anger,fear,love . This is a Natural language Processing based problem where i done tokenization,lemmitization and trained with processed keywords to achieve the model. I've used Hugging NLP package and used the emotion dataset to create the model.

<br />
###Procedure:
1. Installing Hugging's face NLP Package and Importing Emotion dataset.
2. Splitted up the dataset into three- Train_data, Cross_validation_data, Test_data
3. Tokenized train_data with Params {num_words = 10000 and oov_taken= UNK}.
4. Performed Exploratory Data analyis of tweets by visualising Histogram plot between no_of_words_in_a_tweet with its frequency.
5. Padded the tokenized tweets with Params { truncating = post, padding = post }.
6. Created a Highly Dense Multilayered Bidirectional LSTM model to winover this Sequence dataset using tensorflow.
7. Monitored the training using Early Stopping Callback.
8. After few trails and hyperparameter tuning (Units for Hidden layers is set to 20) , the model gave its best performance for the validation set.
9. Then test the model and found its test_data loss to be around 0.44 .
 
