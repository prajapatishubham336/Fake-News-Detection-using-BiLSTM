# Fake-News-Detection-using-BiLSTM
This project implements a Fake News Detection system using Natural Language Processing (NLP) and a Bidirectional Long Short-Term Memory (BiLSTM) neural network.  The model is trained on the WELFake Dataset containing more than 72,000 news articles and is capable of classifying news articles as Real or Fake.


## Project Overview

This project implements a Fake News Detection system using Natural Language Processing (NLP) and a Bidirectional Long Short-Term Memory (BiLSTM) neural network.

The model is trained on the WELFake Dataset containing more than 72,000 news articles and is capable of classifying news articles as Real or Fake.

---

## Dataset

Dataset: WELFake Dataset

Total Records: 72,095

Class Distribution:

* Fake News (Label = 1): 37,106
* Real News (Label = 0): 35,028

After preprocessing:

* Total Records Used: 72,095

---

## Data Preprocessing

The following preprocessing steps were applied:

* Convert text to lowercase
* Remove URLs
* Remove HTML tags
* Remove numbers
* Remove punctuation
* Remove extra whitespace

---

## Model Architecture

Embedding Layer

↓

Bidirectional LSTM (32 Units)

↓

Dense Layer (ReLU)

↓

Dropout (0.3)

↓

Output Layer (Sigmoid)

---

## Training Configuration

| Parameter           | Value  |
| ------------------- | ------ |
| Vocabulary Size     | 15,000 |
| Max Sequence Length | 200    |
| Batch Size          | 128    |
| Epochs              | 5      |
| Optimizer           | Adam   |
| Learning Rate       | 0.001  |

---

## Results

### Test Accuracy

96.54%

### Classification Report

| Metric    | Score     |
| --------- | --------- |
| Precision | 96% - 97% |
| Recall    | 96% - 97% |
| F1 Score  | 96% - 97% |

### Confusion Matrix

```text
[[6713 293]
 [206 7207]]
```



## Technologies Used

* Python
* TensorFlow / Keras
* Pandas
* NumPy
* Scikit-Learn
* Google Colab

---


## Future Improvements

* DistilBERT-based Fake News Detection
* BERT Fine-Tuning
* Streamlit Web Application
* Explainable AI Integration

---

## References

### Dataset

WELFake Dataset

https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification

### Documentation

TensorFlow:
https://www.tensorflow.org/

Keras:
https://keras.io/

Scikit-Learn:
https://scikit-learn.org/

Pandas:
https://pandas.pydata.org/

Machine Learning & Deep Learning Projects
