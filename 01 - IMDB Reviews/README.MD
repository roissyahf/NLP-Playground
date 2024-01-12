## Classify IMDB Reviews with Deep Learning

This repository documents my experiments in classifying IMDB user review into 2 classes: positive and negative using RNN and LSTM.

### Approach

1. Text Processing and EDA
2. Splitting and sampling the data
3. Text Vectorization
4. Embedding Layer
5. Modeling with Simple RNN, Deep NN
6. Modeling with Global Average Pooling 1D
7. Modeling with Simple LSTM, Single Bidirectional, Multi Bidirectional, add argument merge_mode to Bidirectional
8. Hyperparameter Tuning: Start simple model add complexity later (number of layer, neuron, model type), Dropout layer, Regularization, Changing (LR, activation function, optimizer), Add more data (using all data instead of its sample).

### Results

Here's the accuracy comparison of some models (without data sampling): 
| Model | Special Treatment | Acc train | Acc test |
| --- | --- | --- | --- |
| Global Average Pooling 1D | Applying kernel regularizer (L1=0.00001, L2 = 0.0005) | 0.9630 | 0.8543 |
| Multibidirectional LSTM | Applying kernel regularizer (L1=0.1, L2 = 0.05) | 0.8796 | 0.8217 |

In this experimentation, I trained model using sample data and all data. The model with sample data is overvitting. While using all data, and implementing regularization technique the model perform better.

### Future Work

Try different model, using pretrained networks perhaps.