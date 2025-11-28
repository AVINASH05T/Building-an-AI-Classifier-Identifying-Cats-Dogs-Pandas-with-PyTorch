#  Building an AI Classifier: Identifying Cats, Dogs & Pandas with PyTorch

---

## Introduction

The goal of this project is to develop an **AI-based image classification model** capable of distinguishing between **cats**, **dogs**, and **pandas** using **PyTorch**.  
By leveraging **transfer learning** from powerful pre-trained models such as **ResNet18** or **VGG16**, the project demonstrates how deep learning can accurately identify animals from images while reducing training time and computational cost.

This project is built as part of a workshop assignment to explore **computer vision**, **GPU acceleration**, and **model deployment** using Python and PyTorch.

---

## Overview

This project involves several key steps:

1. **Environment Setup**  
   - Verifying Python and PyTorch installation  
   - Ensuring GPU (CUDA) availability  

2. **Data Preparation**  
   - Using the *Cats, Dogs, and Pandas Dataset* from Kaggle  
   - Organizing data into structured folders for training and testing  
   - Applying data transformations (resize, normalization, augmentation)  

3. **Model Design**  
   - Using transfer learning with a pre-trained model (ResNet18/VGG16)  
   - Replacing the classifier head for 3-class classification (cat, dog, panda)  

4. **Model Training**  
   - Training with Adam optimizer and CrossEntropyLoss  
   - Running for 10–15 epochs  
   - Saving the best-performing model  

5. **Model Evaluation**  
   - Evaluating accuracy and loss on test data  
   - Displaying confusion matrix and example predictions  

6. **(Optional) Deployment**  
   - Deploy the model using Streamlit or Flask to classify new images interactively.  

---

##  Project Structure

Building-an-AI-Classifier-Identifying-Cats-Dogs-Pandas-with-PyTorch/
│
├── AVINASH_AI_classifier_.ipynb # Main Jupyter Notebook with full code
├── README.md # Project documentation
├── requirements.txt # List of required dependencies
└── data/ # Dataset directory (after download)
├── train/
│ ├── cat/
│ ├── dog/
│ └── panda/
└── test/
├── cat/
├── dog/
└── panda/

## Model Overview

Base Model: ResNet18 / VGG16 (Transfer Learning)

Classifier Head:

Fully Connected Layer (256 neurons, ReLU, Dropout 0.5)

Output Layer (3 neurons → Cat, Dog, Panda)

Loss Function: CrossEntropyLoss

Optimizer: Adam (lr=0.001)

Epochs: 10–15

Metric: Accuracy


## Conclusion

This project demonstrates the complete pipeline of building a multi-class image classifier using PyTorch, from data preprocessing to model evaluation.
It showcases the power of transfer learning and provides a strong foundation for future projects involving AI and computer vision.
