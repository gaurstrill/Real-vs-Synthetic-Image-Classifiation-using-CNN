## Real vs Synthetic Image Classification using CNN

This project involves the development of a machine learning model that classifies images as either real or synthetic. The dataset used for training and evaluation is obtained from CIFAKE: Real and AI-Generated Synthetic Images on Kaggle. The dataset consists of 50,000 images each for training of both real and synthetic images, and the test set contains 10,000 images of each category.

### Evaluation Metrics
The model's performance is evaluated using the following metrics:
- F1-score
- Precision
- Accuracy
- Confusion Matrix

### Evaluation Results
The evaluation results for the model are as follows:

| Class            | Precision | Recall  | F1-Score | Support |
|------------------|-----------|---------|----------|---------|
| Real Images      | 0.86      | 0.88    | 0.87     | 10,000  |
| Synthetic Images | 0.88      | 0.85    | 0.87     | 10,000  |
| Accuracy         |           |         | 0.87     | 20,000  |

### Model Summary

The model architecture is a sequential CNN with the following layers:

| Layer (type)    | Output Shape        | Param # |
|-----------------|---------------------|---------|
| conv2d          | (None, 32, 32, 64)  | 1792    |
| conv2d_1        | (None, 32, 32, 64)  | 36928   |
| max_pooling2d   | (None, 16, 16, 64)  | 0       |
| conv2d_2        | (None, 16, 16, 32)  | 18464   |
| conv2d_3        | (None, 16, 16, 32)  | 9248    |
| max_pooling2d_1 | (None, 8, 8, 32)    | 0       |
| conv2d_4        | (None, 8, 8, 16)    | 4624    |
| conv2d_5        | (None, 8, 8, 16)    | 2320    |
| max_pooling2d_2 | (None, 4, 4, 16)    | 0       |
| flatten         | (None, 256)         | 0       |
| dense           | (None, 8)           | 2056    |
...

Total params: 75,478

Trainable params: 75,478

Non-trainable params: 0


Please ensure that you have the necessary dependencies installed before running the project.

Feel free to customize the README file as per your requirements and project structure.
