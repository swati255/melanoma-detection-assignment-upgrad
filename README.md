# melanoma-detection-assignment-upgrad

In this assignment, you will build a __multiclass classification model using a custom convolutional network in TensorFlow__.

## Problem statement:
To build a CNN based model which can accurately detect __melanoma__. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the __International Skin Imaging Collaboration (ISIC)__. All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

### NOTE:
- You don't have to use any pre-trained model using Transfer learning. All the model building processes should be based on a custom model.
- Some of the elements introduced in the assignment are new, but proper steps have been taken to ensure smooth learning. You must learn from the base code provided and implement the same for your problem statement.
- The model training may take time to train as you will be working with large epochs. It is advised to use GPU runtime in Google Colab.

## Project Pipeline
- __Data Reading/Data Understanding__ -> Defining the path for train and test images
- __Dataset Creation__ -> Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- __Dataset visualisation__ -> Create a code to visualize one instance of all the nine classes present in the dataset
- __Model Building & training:__
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale the images to normalize pixel values between (0, 1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit. You must check if there is any evidence of model ovefit ot underfit
- __Choose an appropriate data augmentation stratergy to resolve underfitting/overfitting__
- __Model Building & training on the augmented data:__
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale the images to normalize pixel values between (0, 1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit, see if the earlier issue is resolved or not?
- __Class distribution:__ Examine the current class distribution in the training dataset
  - Which class has the least number of samples?
  - Which classes dominate the data in terms of the proportionate number of samples?
- __Handling class imbalance:__ Rectify class imbalance present in the training dataset with Augmentor library.
- __Model Building & training on the rectified class imbalance data:__
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale the images to normalize pixel values between (0, 1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~30 epochs
  - Write your findings after the model fit, see if the issues are resolved or not?


