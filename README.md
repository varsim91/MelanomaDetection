#  Melanoma Detection 
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis



## Table of Contents
- [Table of Contents](#table-of-contents)
- [General Information](#general-information)
- [Conclusions](#conclusions)
- [Technologies Used](#technologies-used)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis

Dataset  can be found [here](https://drive.google.com/file/d/1xLfSQUGDl8ezNNbUkpuHOYvSpTyxVhCs/view)

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

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

By using the provided images of diseases, we want to build a CNN model which can accurately detect 9 classes present in the dataset. 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

Initial model iterations exhibited significant overfitting. To address this, several optimization techniques were implemented. First, `DropLayer` and `BatchNormalization` layers were incorporated into the architecture, which successfully reduced overfitting but resulted in decreased model accuracy.

Subsequently, data augmentation techniques were applied to expand the training dataset. While this further mitigated overfitting, it did not yield improvements in model accuracy. The most effective intervention proved to be class rebalancing, which substantially reduced both overfitting and loss metrics.

Despite these iterative improvements in the model architecture and training approach, the final model accuracy remains at approximately 60%, indicating room for further optimization.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- tensorflow: 2.17.0
- matplotlib: 3.8.4
- numpy: 1.26.4
- keras: 3.6.0
- pandas: 2.2.2
<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- Inspired by IIITB CNN assignment
- Credit to IIITB and Upgrad


## Contact
Created by [@varsim91] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
