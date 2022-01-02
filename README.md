# comment-verification
This is the final project of artificial intelligence course fall 2019. 

## Description
In this project I implemented a spam detection model using different
machine learning models, LSTM-based models, and BERT model. The data is from digikala contest, and it consists of comments made by users. 

## Dataset
This dataset has 160000 records for train and 20000 records for test.

Here are the link to my dataset:

train dataset : [link](https://drive.google.com/file/d/18PSMJoPB_j45zGVOnCmryKLSJhw0_htI/view?usp=sharing)

test dataset : [link](https://drive.google.com/file/d/17vm0BbuJUrYCAIqB-anVhKFqNPSirlNL/view?usp=sharing)

## Machine Learning models

I used LogisticRegression and MultinomialNB for classification. Also, TF-IDF is used for the embedding. The models trained using all the train data.

| LogisticRegression Accuracy  | MultinomialNB Accuracy |
| ------------- | ------------- |
| 87% | 89%  |

## Deep Learning models

I implemented BILSTM, BIGRU with and without attention layer. The models trained using 8000 records of the train data.

| BILSTM Accuracy  | BILSTM with attention Accuracy | BIGRU Accuracy  | BIGRU with attention Accuracy |
| ------------- | ------------- | ------------- | ------------- |
| 87% | 88%  | 85% | 82%|


## Fine-tuned BERT

I fine-tuned the PARSBERT model by adding two linear layer, dropout layer, activation function, and a softmax layer. The model trained using 8000 records of the train data.

| Fine-tuned BERT Accuracy  |
| ------------- |
| 78% |
