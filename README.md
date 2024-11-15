# Leaf Disease Classification using EfficientNetB3

This repository contains a deep learning project focused on identifying and classifying diseases in plant leaves using the EfficientNetB3 model. The model is trained on an extensive dataset of leaf images representing multiple disease categories to help accurately diagnose plant diseases and support effective crop management.

## Features

- **Model Architecture**: Utilizes EfficientNetB3 for its balance of accuracy and efficiency, achieving robust performance on leaf disease classification tasks.
- **Dataset and Preprocessing**: Includes data preprocessing techniques such as image resizing, normalization, and data augmentation to improve model generalization and handle varied lighting conditions.
- **Training Pipeline**: The training script leverages TensorFlow/Keras, including training strategies like early stopping and learning rate reduction for optimized convergence.
- **Evaluation Metrics**: Supports various metrics (accuracy, F1 score, etc.) to assess model performance on unseen data.

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/rronak818/Leaf_Disease_Classification_Using_EfficientNetB3.git
cd leaf-disease-classification
pip install -r requirement.txt
```

## Dataset

The dataset used for training and evaluating the model can be downloaded from Kaggle. You can get the "New Plant Diseases Dataset" from the following link:

- [New Plant Diseases Dataset](https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset)

  This dataset is recreated using offline augmentation from the original dataset. The original dataset can be found on this github repo. This dataset consists of about 87K rgb images of healthy and diseased crop leaves which is categorized into 38 different classes. The total dataset is divided into 80/20 ratio of training and validation set preserving the directory structure. A new directory containing 33 test images is created later for prediction purpose.


## Usage

Train, Evaluate, and Test the Model:

Open the train.ipynb Jupyter Notebook and run the cells to train the EfficientNetB3 model, evaluate its performance, and test it on the test dataset. The notebook includes all necessary code and steps for these tasks.

```bash
jupyter notebook train.ipynb
```

The notenook is structured to:

- Load and preprocess the dataset.
- Train the model.
- Evaluate the model on the validation and test datasets.
- Display performance metrics and results.

## Results and Analysis

The model achieves an accuracy of ~98% on the test dataset. Detailed evaluation metrics and results are displayed directly in the train.ipynb notebook.

- Training VS Validation PLot:

    ![Train vs validation plot](images/plot.png)


- Classification Report:

    ![Classificatin Report](images/report.png)

## Contributing

Feel free to open issues, submit PRs, or discuss improvements to the model and repository structure.

## Licence

This project is licensed under the MIT License. See the LICENSE file for details.
  
