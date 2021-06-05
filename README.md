# Image Classification of Scenes Based on VGG-16 Network Architecture and Transfer Learning
## Introduction to notebooks
There are two notebooks in this repository:
1. intel_image_classification_own_training.ipynb - Classifier with VGG16 network (trained from scratch). 
2. intel_image_classification_transfer_learning.ipynb - Classifier with fintuning a pretrained VGG16 network.

Both of the notebooks has the sections:
Section 1: Setup Parameters and Variables
Section 2: Learning on VGG16 architecture
Section 3: Loss Functions and Optimizers
Section 4: Train Classifier
Section 5: Classify Images

## Environment Setup and Dataset
You can download the dataset used in this project at: https://www.kaggle.com/puneet6060/intel-image-classification
The dataset has only train and test folders. In order to run the codes, please separate create a "seg_val" folder and put 3K images into the folder from "seg_test" folder. Load the data folder and files into your google drive.

### Mounting Google Drive
In order to mount the google drive into collab, please follow the steps here: https://colab.research.google.com/notebooks/io.ipynb

After mounting the drive, need to update the variables in "Section: Setup Parameters and Variables": training_dir, validation_dir, testing_dir to match your folder structure.

### Turn on GPU Mode
Since the model has been setup to run on GPUs, the collab notebook needs to be in GPU mode. 
Go to Runtime > Change Runtime > Select "GPU" as hardware accelerator.

