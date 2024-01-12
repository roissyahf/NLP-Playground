## Classify BBC News Category with Machine Learning and Deep Learning

This repository documents my experiments in classifying BBC News into 5 category: sport, business, politics, entertainment, and tech. Machine Learning model used are Naive Bayes, Decision Tree, and Random Forest, meanwhile in Deep Learning the model used is just RNN.

### Approach

1. Encode the label category
2. Text processing
3. Model Training
4. Model Evaluation
5. Prediction

### Results

Here's the accuracy comparison of the model used: 
| Model | Acc train | Acc val |
| --- | --- | --- |
| Naive Bayes | 99.161 | 96.644 |
| Decision Tree | 99.161 | 81.543 |
| Random Forest | 99.161 | 95.973 |
| Global Average Pooling 1D | 0.9961 | 0.9414 |

From above table we can conclude that Deep Learning surpass Machine Learning model, but this is not the final conclusion we can made.

### Future Work

Tuning the hyperparameter.