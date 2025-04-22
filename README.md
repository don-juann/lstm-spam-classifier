# LSTM - Deep Learning Spam Classifier model
## Overview
This project demonstrates utilizing LSTM (Long-Short Term Memory) Deep Learning model, which is a more advanced version of RNN (Recurrent Neural Network), to detect a spam message using SMS Spam Collection Dataset.

### Preprocessing Data
1. Cleaning data, removing nonfunctional columns
2. Renaming columns
3. Using LabelEncoding to encode target variable  
4. Splitting data into training, validation and testing sets
5. Tokenizing text, so model can take it as input:
- Vocabulary size = 5000
- Maximum length = 100

### Training Process
1. Creating model - LSTM: 
- Embedding layer: (output_dim = 128)
- Bidirectional layer, LSTM layer: (64, dropout = 0.2, recurrent_dropout = 0.2)
- Dense layer: (1, activation='sigmoid')
2. Training for 10 epochs
  
3. Metrics:
- Accuracy: 0.9904306220095693  
- Precision: 0.9905660377358491  
- Recall: 0.9375  
- F1 Score: 0.963302752293578
4. Inference results:
- Spam example: Spam probability - 100%, Predicted label - Spam
- Ham example: Spam probability - 0%, Predicted label - Ham

### Results
As a result, a LSTM model was created using sms-spam-collection-dataset taken 
from Kaggle. Although model managed to reach great performance result of 99%, it might be improved even further by applying various regularization techniques such as 
augmentation, early stopping and etc. 
Model also has shown itself to be great at unseen data, which was demonstrated in inference testing. Overall, great work has been done to solve Natural Language Processing task such as text classification, 
to be more precise - spam classification task.

## Acknowledgement
Dataset - SMS Spam Collection Dataset provided by UCI Machine Learning.
- Zhan Kazikhanov
- jkazikhanov@gmail.com
- github.com/don-juann
