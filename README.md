# CS410HW3

**Problem 1
**
When comparing model performance with and without stopwords, the version excluding stopwords resulted in a slightly lower and more consistent RMSE distribution. The histogram showed a sharper concentration around lower RMSE values, which suggests better prediction accuracy. Therefore, set the flag to FALSE. 

**Problem 2
**

BERT Accuracy: 0.004868421052631579
GPT-2 Accuracy: 0.23763157894736842

GPT-2 outperformed BERT on next-word prediction, with an accuracy of about 23.76%.

BERT’s accuracy, approximately 0.49%, is low but expected, as it is not optimized for predicting the next word, since it is not a generative model.

This result supports the idea that autoregressive models like GPT-2 are better suited for next-word prediction tasks, while BERT excels in tasks like classification, fill-in-the-blank, or QA.

**Problem 3
**

<img width="798" alt="Screenshot 2025-05-05 at 7 45 46 PM" src="https://github.com/user-attachments/assets/23968cad-9758-4065-8c13-b9192335b227" />

Top 5 terms:
new: 0.0067
first: 0.0062
last: 0.0053
presidential: 0.0047
one: 0.0047

**Problem 4
**

TRAINING CLASSIFICATION REPORT:
              precision    recall  f1-score   support

           0       0.75      1.00      0.86         3
           1       1.00      0.67      0.80         3

    accuracy                           0.83         6
   macro avg       0.88      0.83      0.83         6
weighted avg       0.88      0.83      0.83         6

TEST CLASSIFICATION REPORT:
              precision    recall  f1-score   support

           0       0.00      0.00      0.00         2
           1       0.33      0.50      0.40         2

    accuracy                           0.25         4
   macro avg       0.17      0.25      0.20         4
weighted avg       0.17      0.25      0.20         4
