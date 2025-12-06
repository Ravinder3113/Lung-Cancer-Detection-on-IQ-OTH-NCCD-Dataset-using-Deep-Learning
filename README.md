# Lung Cancer CT Scan Classification using AlexNet

This repository presents a complete deep learning pipeline for classifying lung cancer using CT scan images. The project includes dataset preprocessing, AlexNet-based model development, training, evaluation, and inference. The goal is to build a reproducible framework demonstrating how convolutional neural networks can support early lung cancer detection.

## Dataset

This project uses the publicly available IQ-OTHNCCD Lung Cancer Dataset from Kaggle:

https://www.kaggle.com/datasets/adityamahimkar/iqothnccd-lung-cancer-dataset

The dataset contains CT scan images categorized into multiple types of lung cancer as well as normal cases.


## Installation

Install the required dependencies:

pip install torch torchvision numpy matplotlib pillow opencv-python

## Running the Project

### 1. Clone the Repository

git clone https://github.com/Ravinder3113/Lung-Cancer-Detection-on-IQ-OTH-NCCD-Dataset-using-Deep-Learning
cd lung-cancer-classification

### 2. Download the Dataset

Download the dataset and place it into:

data/train/
data/test/

### 3. Open the Jupyter Notebook

jupyter notebook DL_Project.ipynb

### 4. Train the Model

Run the training cells in the notebook to train the AlexNet-based model.

### 5. Perform Inference

Use the inference section to classify new CT scan images.

## Model Architecture

A modified AlexNet architecture is used for multi-class lung cancer classification. It consists of:

- Convolutional layers with ReLU activation
- Max pooling layers
- Fully connected classifier
- Softmax output

The model is trained using Adam optimizer and cross-entropy loss.

## Data Preprocessing

Image preprocessing and augmentation steps include:

- Resizing
- Normalization
- Random rotations
- Horizontal and vertical flips
- Tensor conversion

These operations help improve generalization and robustness.

## Evaluation

The notebook provides:

- Training and validation accuracy
- Loss curves
- Confusion matrix
- Example predictions

These evaluation tools help measure model performance and reliability.

## Future Improvements

Possible extensions include:

- Adding Grad-CAM for model interpretability
- Testing advanced architectures like ResNet, DenseNet, or EfficientNet
- Using 3D CNNs for volumetric CT scan analysis
- Deploying the model using Flask or FastAPI

## License

This project is released under the MIT License.
