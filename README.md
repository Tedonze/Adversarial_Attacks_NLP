"# Adversarial ATTACK DETECTION " 

In this jupyter notebook we have built three methods of out of distribution detection:

- Max-softmax
- Doctor discriminator, 
- Mahanobis distance 

As metrics we have used:
- AUROC
- AUPR

We build a Sentiment classifier using a pretrained model (You can choose bert or Robert),
and we train it on different dataset (imdb,ag-news,sst2).

Then we use a text attack generator according to this repository https://github.com/bangawayoo/adversarial-examples-in-text-classification

(we have put some generated attacks file in the attack foler)

Then we compute each metrics to evaluate ODD detection


To test different scenario we provide at the top of our notebook a config file as global variable
###### Global Variable 
PRE_TRAINED_MODEL_NAME = 'bert-base-cased' #'robbert-base-cased'
PATH_to_attack_data="/content/drive/MyDrive/adversarial-examples-in-text-classification/imdb__textattackbert-base-uncased-imdb_bert__pwws.csv"
PATH_to_saved_model="/content/drive/MyDrive/cache/best_model_state.bin"
