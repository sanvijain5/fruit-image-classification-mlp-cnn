# Fruit Image Classification Using MLP and CNN

**Author:** Sanvi Jain  
**Course:** Neural Networks and Deep Learning  
**Project:** Academic deep-learning assignment

## Overview

This project implements and compares neural-network approaches for multi-class fruit image classification using a subset of the Fruits-360 dataset:

- **MLP (Multilayer Perceptron):** flattens image pixels before classification.
- **CNN (Convolutional Neural Network):** learns spatial image features through convolution and pooling.
- **Improved CNN:** experiments with additional convolutional layers, data augmentation, and dropout.

## Objectives

- Preprocess fruit images and inspect sample data.
- Train MLP and CNN models using TensorFlow/Keras.
- Plot training vs. validation accuracy and loss.
- Generate a confusion matrix.
- Compare test accuracy/loss, training time, and model parameter counts.
- Explore techniques intended to improve generalization.

## Repository contents

- `fruit_classification_mlp_cnn.ipynb` — notebook with code, outputs, visualizations, and explanations.
- `requirements.txt` — Python package dependencies.
- `results/` — optional exported plots and screenshots can be added here.

## Dataset

Use the Fruits-360 dataset or the subset supplied for the course assignment.

- Official project: https://github.com/fruits-360/fruits-360
- The dataset is not included in this repository. Please review the dataset's terms/licence before downloading or redistributing it.

Expected folder structure:

```text
fruitsDataset/
├── Training/
│   ├── class_name_1/
│   ├── class_name_2/
│   └── ...
└── Test/
    ├── class_name_1/
    ├── class_name_2/
    └── ...
```

## Run in Google Colab

1. Upload the notebook to Google Colab.
2. Upload or mount your dataset in the Colab runtime.
3. Ensure the folders are available at `/content/fruitsDataset/Training` and `/content/fruitsDataset/Test`, or update `train_path` and `test_path` in the notebook.
4. Run the notebook cells in order.

The notebook includes Google Drive mounting and archive-extraction cells from the original workflow. If your dataset is already extracted, skip the archive-extraction step.

## Results and interpretation

The notebook contains training/validation curves, a confusion matrix, model parameter counts, and test evaluation. Re-run the notebook in your own environment before quoting exact results in a CV or public post.

**Important evaluation note:** The recorded runs show a substantial gap between training and validation performance. Before treating metrics as final, verify the validation pipeline, ensure augmentation is applied only to training data, and use the same held-out test set for all model comparisons. The confusion matrix should be generated from the intended evaluation split with matching class indices.

## Technologies

Python · TensorFlow/Keras · NumPy · Matplotlib · Seaborn · Scikit-learn · Jupyter Notebook

## Skills demonstrated

Deep learning fundamentals, image preprocessing, multi-class classification, CNN architecture, model evaluation, data visualization, and comparative experimentation.
