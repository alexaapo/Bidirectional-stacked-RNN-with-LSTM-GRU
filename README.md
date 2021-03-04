# Bidirectional stacked RNN with LSTM GRU

Here I develop a sentiment classifier using a ***bidirectional stacked RNN with LSTM/GRU cells*** for the Twitter sentiment analysis dataset, which is [available here](https://drive.google.com/file/d/1dTIWNpjlrnTQBIQtaGOh0jCRYZiAQO79/view).  

For the development of the models, I experimented with the number of stacked RNNs, the number of hidden layers, type of cells, skip connections, gradient clipping and dropout probability. I use the Adam optimizer and the binary cross-entropy loss function and I transformed the predicted logits to probabilities using a sigmoid function. 

For the best model I found:
* Compute precision, recall and F1 for each class.
* Plot the loss vs epochs curve and the ROC curve 

My solution is implemented in ***PyTorch*** and the report is well documented. I also have a notebook with the preprocess of the data.

***Note:*** I also utilize pre-trained word embeddings ***GloVe*** as the initial embeddings to input on your models.
