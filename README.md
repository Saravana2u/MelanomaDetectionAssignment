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
####  The data set contains the following 9 class diseases
- &nbsp;&nbsp;&nbsp;&nbsp;  1) Actinic keratosis
- &nbsp;&nbsp;&nbsp;&nbsp;  2) Basal cell carcinoma
- &nbsp;&nbsp;&nbsp;&nbsp;  3) Dermatofibroma
- &nbsp;&nbsp;&nbsp;&nbsp;  4) Melanoma
- &nbsp;&nbsp;&nbsp;&nbsp;  5) Nevus
- &nbsp;&nbsp;&nbsp;&nbsp;  6) Pigmented benign keratosis
- &nbsp;&nbsp;&nbsp;&nbsp;  7) Seborrheic keratosis
- &nbsp;&nbsp;&nbsp;&nbsp;  8) Squamous cell carcinoma
- &nbsp;&nbsp;&nbsp;&nbsp;  9) Vascular lesion
####  Assignment Steps 
- &nbsp;&nbsp;&nbsp;&nbsp; 1) Data Reading/Data Understanding 
- &nbsp;&nbsp;&nbsp;&nbsp; 2) Dataset Creation
- &nbsp;&nbsp;&nbsp;&nbsp; 3) Dataset visualisation
- &nbsp;&nbsp;&nbsp;&nbsp; 4) Basic CNN Model Building and Validation
- &nbsp;&nbsp;&nbsp;&nbsp; 5) Data augmentation strategy to resolve underfitting/overfitting 
- &nbsp;&nbsp;&nbsp;&nbsp; 6) CNN Model with Dropout, Batch Normalization, l2 Regularization along with more CNN layers
- &nbsp;&nbsp;&nbsp;&nbsp; 7) Class distribution Study
- &nbsp;&nbsp;&nbsp;&nbsp; 8) Handling class imbalances using  Augmentor library
- &nbsp;&nbsp;&nbsp;&nbsp; 9) Model Building & training on the rectified class imbalance data after Augmentation
- &nbsp;&nbsp;&nbsp;&nbsp;  10) Conclusions


## Conclusions
#### Conclusion 1 :
- &nbsp;&nbsp;&nbsp;&nbsp;    This first basic CNN model is overfit model.
- &nbsp;&nbsp;&nbsp;&nbsp;    Training accuracy is : 0.9125
- &nbsp;&nbsp;&nbsp;&nbsp;    Validation accuracy is : 0.3898 almost constant on each Epoch and it does not improve¶
- &nbsp;&nbsp;&nbsp;&nbsp;    Training accuracy very high compared to validation accuracy which means that the model memorized the training data but failed to predict the test data
- &nbsp;&nbsp;&nbsp;&nbsp;    Validation loss is increasing for each Epoch and it should reduce for a good CNN model
- &nbsp;&nbsp;&nbsp;&nbsp;    This is not a good CNN model for Melanoma Detection
#### Conclusion 2 :
- &nbsp;&nbsp;&nbsp;&nbsp;   This second CNN model with Dropout, Batch Normalization, l2 Regularization and more CNN layers is also overfit model.
- &nbsp;&nbsp;&nbsp;&nbsp;   Training accuracy is : 0.8566
- &nbsp;&nbsp;&nbsp;&nbsp;   Validation accuracy is : 0.3559 wich is improved slightly and becomes constant
- &nbsp;&nbsp;&nbsp;&nbsp;   Training accuracy very high compared to validation accuracy which means that the model memorized the training data but failed to predict the test data
- &nbsp;&nbsp;&nbsp;&nbsp;   Validation loss is decreasing for each Epoch and it is a good sign and more Epochs may help to improve the CNN model
- &nbsp;&nbsp;&nbsp;&nbsp;   This second CNN model also not a good model for Melanoma Detection
- &nbsp;&nbsp;&nbsp;&nbsp;   The diseases classes are having highly imbalance data which resulted in poor CNN Model
#### Conclusion 3 :
- &nbsp;&nbsp;&nbsp;&nbsp;    This final CNN model with Data Augmentation, Dropout, Batch Normalization, l2 Regularization and with more CNN layers is a good CNN model.
- &nbsp;&nbsp;&nbsp;&nbsp;    Training accuracy is : 0.9283
- &nbsp;&nbsp;&nbsp;&nbsp;    Validation accuracy is : 0.8322
- &nbsp;&nbsp;&nbsp;&nbsp;    Training accuracy and Validation Accuracy is steadily increasing for each Epoch¶
- &nbsp;&nbsp;&nbsp;&nbsp;    Training loss and Validation loss is steadily decreasing for each Epoch
- &nbsp;&nbsp;&nbsp;&nbsp;    Data augmentation and handling class imbalance helped to achive this good model
- &nbsp;&nbsp;&nbsp;&nbsp;    This final CNN model is a good model for Melanoma Detection

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
