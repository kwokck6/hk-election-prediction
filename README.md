# Hong Kong Election Predictions
## Purpose
- To provide predictions given the socio-economic indices from the census only.
- To visualise political polarity in different kinds of living environments, e.g. rural and urban, less-developed and higher-developed areas.
- To encourage the use of AI for social betterment.

## Methodology
### Method 1: Use simple machine learning models
1. Preprocessing of data:
   1. Clean the census data, e.g. replace '\*', '\*\*' and '-' to 0 and remove NAs.
   2. Calculate the plurality winner from the counting station, and label the corresponding DCCA.
   3. Retain the DCCA that exists from both 2012 and 2016 
2. Predict before feature extraction.
3. Do feature extraction according to chi-squared distribution.
4. Predict (as a comparison) after feature extraction.

### Method 2A: Use Graph Neural Networks
To do.

### Method 2B: Use Hierarchical GNN
To do. An advanced verson of Method 2A.

## Results
### Method 1
Does not perform well: perform as badly as random. Table below shows the performance for predicting among 17 political party.

|         Model         | Before |  After |
|-----------------------|--------|--------|
|     Decision Tree     | 35.43% | 35.43% |
|     Random Forest     | 37.53% | 36.22% |
|          LDA          | 34.65% | 25.98% |
|          QDA          | 33.33% | 33.33% |
|  Logistic Regression  | 28.87% | 22.31% |
| Multilayer Perceptron | 32.55% | 51.97% |

### Method 2A
To do.

### Method 2B
To do.
