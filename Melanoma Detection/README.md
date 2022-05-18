# Melanoma Detection
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Analysis approach
- Data Reading/Data Understanding → Defining the path for train and test images 
- Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset 
- Model Building & training : 
        Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
        Choose an appropriate optimiser and loss function for model training
        Train the model for ~20 epochs
- Data Augmentation: Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
- Model Building & training on the augmented data :
        Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
        Choose an appropriate optimiser and loss function for model training
        Train the model for ~20 epochs
- Class distribution: Examine the current class distribution in the training dataset 
- Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library.
- Model Building & training on the rectified class imbalance data :
        Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
        Choose an appropriate optimiser and loss function for model training
        Train the model for ~30 epochs
 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Data augmentation improves the accuracy.
- Generating more images helps in increasing the training and validation accuracy.
- Using dropouts helps in avoiding overfitting.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- tensorflow
- pathlib
- numpy
- pandas
- os
- PIL
- matplotlib.pyplot
- tensorflow.keras
- tensorflow.keras.models
- tensorflow.keras.optimizers
- kears.callbacks
<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was based on [this tutorial](https://www.tensorflow.org/tutorials/images/classification).


## Contact
Created by [@idhaya-r] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->