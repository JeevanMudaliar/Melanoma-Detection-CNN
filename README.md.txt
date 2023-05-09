Melanoma Detection using Convolutional Neural Network Model

Melanoma is a type of cancer that can be fatal if not detected early, accounting for 75% of skin cancer deaths. To address this problem, we aim to build a CNN-based model that can accurately detect melanoma from images, potentially reducing the manual effort required for diagnosis.

The dataset used in this project consists of 2357 images of malignant and benign oncological diseases, sorted according to the classification taken with the International Skin Imaging Collaboration (ISIC). The dataset includes nine classes, including Actinic keratosis, Basal cell carcinoma, Dermatofibroma, Melanoma, Nevus, Pigmented benign keratosis, Seborrheic keratosis, Squamous cell carcinoma, and Vascular lesion.
Our business goal is to build a multiclass classification model using a custom convolutional neural network in TensorFlow. The potential business risk is predicting an incorrect class of skin cancer, which could lead to misdiagnosis and inadequate treatment.

The project pipeline includes several stages, starting with data reading and understanding, creating a dataset from the train directory, and visualizing the data. Next, we build and train a CNN model with an appropriate optimizer and loss function, using an appropriate data augmentation strategy to resolve underfitting or overfitting.
We examine the current class distribution in the training dataset and identify the class with the least number of samples, as well as the classes that dominate the data in terms of the proportionate number of samples. We use the Augmentor library to rectify class imbalances present in the training dataset.

Finally, we build and train a CNN model on the rectified class imbalance data, using an appropriate optimizer and loss function, and train the model for approximately 30 epochs. We record our findings after each model fit, checking for evidence of overfitting or underfitting, and assessing whether the earlier issues have been resolved or not.
