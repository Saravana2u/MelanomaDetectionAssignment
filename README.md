# Project Name -Melanoma Detection Assignment -   By Saravanakumar PERUMAL
> Description : 
    In this assignment, multiclass classification CNN model is built using a custom convolutional neural network in TensorFlow. 
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information

- Problem statement: To build a CNN based model which can accurately detect melanoma. 
- Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
- The data set contains the following 9 clas diseases
    : 1) Actinic keratosis
    : 2) Basal cell carcinoma
    : 3) Dermatofibroma
    : 4) Melanoma
    : 5) Nevus
    : 6) Pigmented benign keratosis
    : 7) Seborrheic keratosis
    : 8) Squamous cell carcinoma
    : 9) Vascular lesion
- Assignment Steps 
    : 1) Data Reading/Data Understanding 
    : 2) Dataset Creation
    : 3) Dataset visualisation
    : 4) Basic CNN Model Building and Validation
    : 5) Data augmentation strategy to resolve underfitting/overfitting 
    : 6) CNN Model with Dropout, Batch Normalization, l2 Regularization along with more CNN layers
    : 7) Class distribution Study
    : 8) Handling class imbalances using  Augmentor library
    : 9) Model Building & training on the rectified class imbalance data after Augmentation
    : 10) Conclusions


## Conclusions
- Conclusion 1 :
    : This first basic CNN model is overfit model.
    : Training accuracy is : 0.9125
    : Validation accuracy is : 0.3898 almost constant on each Epoch and it does not improve¶
    : Training accuracy very high compared to validation accuracy which means that the model memorized the training data but failed to predict the test data
    : Validation loss is increasing for each Epoch and it should reduce for a good CNN model
    : This is not a good CNN model for Melanoma Detection
- Conclusion 2 :
    : This second CNN model with Dropout, Batch Normalization, l2 Regularization and more CNN layers is also overfit model.
    : Training accuracy is : 0.8566
    : Validation accuracy is : 0.3559 wich is improved slightly and becomes constant
    : Training accuracy very high compared to validation accuracy which means that the model memorized the training data but failed to predict the test data
    : Validation loss is decreasing for each Epoch and it is a good sign and more Epochs may help to improve the CNN model
    : This second CNN model also not a good model for Melanoma Detection

- Conclusion 3 :
     : This final CNN model with Data Augmentation, Dropout, Batch Normalization, l2 Regularization and with more CNN layers is a good CNN model.
    : Training accuracy is : 0.9283
    : Validation accuracy is : 0.8322
    : Training accuracy and Validation Accuracy is steadily increasing for each Epoch¶
    : Training loss and Validation loss is steadily decreasing for each Epoch
    : Data augmentation and handling class imbalance helped to achive this good model
    : This final CNN model is a good model for Melanoma Detection

## Technologies Used
- python 3 - Jupyter Note Book
- numpy library - version 1.26.4
- pandas library - version 2.2.1
- matplotlib library - version 3.8.3
- plotly library - version 5.22.0
- tensorflow - version 2.18.0
## Acknowledgements

- This project and the data was provided by [IIITB](https://www.iiitb.ac.in/) & [upGrad](https://www.upgrad.com/) learning platform for CNN case study.


## Contact
- Created by [Saravanakumar PERUMAL](https://github.com/Saravana2u/)- feel free to contact me!
- This project work repository is here : [Melanoma Detection CNN Assignment](https://github.com/Saravana2u/MelanomaDetectionAssignment).
