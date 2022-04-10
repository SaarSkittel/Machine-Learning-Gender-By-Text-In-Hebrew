# Machine-Learning-Gender-Classification-By-Text-In-Hebrew
## Introduction

This project was a final project in ML course. The project classify the gender of the composer of a given text in Hebrew.

The project is written in Python using Jupiter Notebook utilizing  Pandas and scikit-learn libraries.
## Work Flow 
### Creating an Dataframe from corpus
Tokenizing the texts using Hebrew tokenizer modified with filtering tokens of words that are not in Hebrew.
Creating stop words file that has most common words in Hebrew who doesn’t indicate the gender of the writer  
### Creating a pipeline:
Vector – from trial and error it seem that count vectorizer works the best in this case with the stop words and tokenizer.

Normailzer- from trial and error it seem that l2 normailzer works the best in this case.

Classifier - using MLPClassifie r(neural networks) with max iterations of 200 , learning rate of 0.01 without shuffle and random state set to 0.

### Train results
Used 80% of the data to train the model and 20% for validation.

              precision    recall  f1-score   support

           f       0.55      0.60      0.57        20
           m       0.84      0.81      0.83        53

    accuracy                           0.75        73
    macro avg      0.69      0.71      0.70        73
    weighted avg   0.76      0.75      0.76        73

### Final results
Used 100% of the data to train the model with a new test results.

              precision    recall  f1-score   support

           f       0.55      0.64      0.59        33
           m       0.88      0.84      0.86       104

    accuracy                           0.79       137
    macro avg      0.72      0.74      0.72       137
    weighted avg   0.80      0.79      0.79       137






