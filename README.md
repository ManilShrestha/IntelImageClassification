# Image Classification of Scenes Based on VGG-16 Network Architecture and Transfer Learning
All the images listed in the paper can be generated through the notebooks in this repository.
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

After mounting the drive, need to update the variables in "Section: Setup Parameters and Variables": training_dir, validation_dir, testing_dir to match your folder structure. Also, update the file path "trained_model_file" where you want the model to be saved in.

### Turn on GPU Mode
Since the model has been setup to run on GPUs, the collab notebook needs to be in GPU mode. 
Go to Runtime > Change Runtime > Select "GPU" as hardware accelerator.

## Train the model
In order to train the model, please run cells in sections 1,2,3, and 4 in order, in section 4 there are multiple optimizers defined, please run the one you want model to be trained on.
Training time depends on the number of epochs defined in the steps. 

## Classify Images
Once the training completes run cells in section 5 to start classifying the images. There are plenty of examples for reference on classifying an image using the trained model.

## Contact
In case of you have questions, please shoot me an email at: ms5267@drexel.edu
