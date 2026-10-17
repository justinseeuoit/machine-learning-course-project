| Model                    |   CV F1 (mean) |   CV F1 (std) |   Train F1 (CV) |   Val Accuracy |   Val Precision |   Val Recall |   Val F1 |   Val ROC-AUC |
|:-------------------------|---------------:|--------------:|----------------:|---------------:|----------------:|-------------:|---------:|--------------:|
| Logistic Regression (L2) |         0      |         0     |          0      |         0.835  |               0 |            0 |        0 |        0.4768 |
| Linear SVM (hinge, L2)   |         0      |         0     |          0      |         0.835  |               0 |            0 |        0 |        0.4758 |
| Perceptron               |         0.1482 |         0.059 |          0.1388 |         0.8325 |               0 |            0 |        0 |        0.5024 |
| Naive (majority class)   |         0      |         0     |          0      |         0.835  |               0 |            0 |        0 |        0.5    |