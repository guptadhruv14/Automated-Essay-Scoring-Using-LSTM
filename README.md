# Automated-Essay-Scoring-Using-LSTM
A Deep Learning model that predicts the score of a given input essay.
The dataset is from Kaggle ASAP competition which was provided by The Hewlett Foundation.

The mysite folder contains the Django app if you want an interactive demo.

Performance
The accuracy is calculated by Quadratic Weighted Kappa(QWK), which measures the agreement between two raters. The state of the art implementation in this competition achieved a QWK score of 0.82 six years ago. My model achieves a QWK score of 0.961. The model architecture consists of 2 Long Short Term Memory(LSTM) layers with a Dense output layer. The final layer uses the Relu activation function. The QWK is calculated by training model on the dataset using 5-Fold Cross Validation and taking the average for all five folds.
