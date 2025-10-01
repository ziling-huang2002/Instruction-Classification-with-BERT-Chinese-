# Instruction Classification with BERT (Chinese)
This repository is part of my coursework for the Kaggle HW1 Instruction Classifier competition. The goal is to classify Chinese instructions into three operation types: replace, insert, and delete. I fine-tuned a BERT-based Chinese pretrained model and incorporated several architectural enhancements to improve classification performance.

## Requirement
Python 3.11.13

## How to Run
Since the dataset is hosted on Kaggle and cannot be redistributed, please follow these steps to run the code directly on the Kaggle platform:
1. Go to the competition page: [HW1 Instruction Classifier](https://www.kaggle.com/competitions/hw-1-instruction-classifier)
2. Click “Join Competition” to gain access to the dataset
3. Download[`main.ipynb`](main.ipynb) from this GitHub repo.
4. On Kaggle, go to “Code” → “New Notebook”.
5. Click “Upload Notebook” and import main.ipynb you just downloaded.
6. Make sure the dataset is correctly mounted under __/kaggle/input/__.
7. Click “Run All” to execute the notebook and generate predictions.

## Result
| Class         | Precision | Recall | F1-Score | Support |
|---------------|----------|-------|----------|--------|
| 0             | 0.943    | 0.971 | 0.957    | 206    |
| 1             | 0.985    | 0.929 | 0.956    | 211    |
| 2             | 0.945    | 0.986 | 0.965    | 140    |
| **Accuracy**  |          |       | 0.959    | 557    |
| **Macro Avg** | 0.958    | 0.962 | 0.959    | 557    |
| **Weighted Avg** | 0.960 | 0.959 | 0.959    | 557    |

![Loss and Accuracy Curve](images/loss_accuracy_curve.png)
![Confusion Matrix](images/bert_confusion_matrix.png)
