# CS410HW3

**Problem 1**

When comparing model performance with and without stopwords, the version excluding stopwords resulted in a slightly lower and more consistent RMSE distribution. The histogram showed a sharper concentration around lower RMSE values, which suggests better prediction accuracy. Therefore, set the flag to FALSE. 

**Problem 2**

BERT Accuracy: 0.004868421052631579

GPT-2 Accuracy: 0.23763157894736842

GPT-2 outperformed BERT on next-word prediction, with an accuracy of about 23.76%.

BERT’s accuracy, approximately 0.49%, is low but expected, as it is not optimized for predicting the next word, since it is not a generative model.

This result supports the idea that autoregressive models like GPT-2 are better suited for next-word prediction tasks, while BERT excels in tasks like classification, fill-in-the-blank, or QA.

**Problem 3**

<img width="798" alt="Screenshot 2025-05-05 at 7 45 46 PM" src="https://github.com/user-attachments/assets/23968cad-9758-4065-8c13-b9192335b227" />

Top 5 terms:

new: 0.0067

first: 0.0062

last: 0.0053

presidential: 0.0047

one: 0.0047

**Problem 4**

<img width="400" alt="image" src="https://github.com/user-attachments/assets/bfba63e3-2710-4ca7-b043-5b6d51d52cd7" />

The report reveals a noticeable difference between training and testing performance, suggesting potential overfitting. While the model achieves 83% accuracy on the training set, its accuracy drops to just 25% on the test set. This implies that the model has memorized the training data but fails to generalize to the unseen examples. Also, the results show that class 0 is completely misclassified (precision and recall of 0.00), indicating the model's bias toward predicting class 1. This issue is supported by the smaller size of the dataset, only 10 documents, which limits the model's ability to learn robust decision boundaries. Overall, the results suggest that the current feature set, comprising PageRank, hub scores, and TF-IDF values, may not be sufficient for effective classification, and the model would benefit from more data or enhanced features.
