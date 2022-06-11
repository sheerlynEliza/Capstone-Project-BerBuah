# Capstone-Project-BerBuah
**CAPSTONE PROJECT BANGKIT 2022** <br/>
In this project, we created a tensorflow model to classify fruit through image processing. We design with 7 classes of fruit, namely: Grapes, Dragon Fruit, Orange, Coconut, Pineapple, Papaya and Strawberry. With this project, we hope that it will be easier for us to recognize various kinds of fruit.

## Project Structure

```bash
.
├── README.md
├── datasets
│   ├── test "--> Our test datasets, contains Anggur, Buah Naga, Jeruk, Kelapa, Nanas, Pepaya, Stroberi"
│   │   ├── Anggur
│   │   ├── Buah Naga
│   │   ├── Jeruk
│   │   ├── Kelapa
│   │   ├── Nanas
│   │   ├── Pepaya
│   │   └── Stroberi
│   ├── train "--> Our train datasets, contains Anggur, Buah Naga, Jeruk, Kelapa, Nanas, Pepaya, Stroberi"
│   │   ├── Anggur
│   │   ├── Buah Naga
│   │   ├── Jeruk
│   │   ├── Kelapa
│   │   ├── Nanas
│   │   ├── Pepaya
│   │   └── Stroberi
│   ├── Validation "--> Our validation datasets, contains Anggur, Buah Naga, Jeruk, Kelapa, Nanas, Pepaya, Stroberi"
│   │   ├── Anggur
│   │   ├── Buah Naga
│   │   ├── Jeruk
│   │   ├── Kelapa
│   │   ├── Nanas
│   │   ├── Pepaya
│   │   └── Stroberi
└── BerBuah.ipynb "--> final python notebook for creating our model"

```

## Dataset
We used [this dataset](https://www.kaggle.com/datasets/ilyasaaffan/iwannafruits) that contains training data, test data and validation data to train our model.

This dataset contains 3600 images (10 fruits), but we only used 7 fruits from 10 fruits in the dataset.
Here are the following lists of 7 fruits that we used

Dataset       | Directories     | Files
------------- | -------------   | -------------
Test          | Anggur          | 10
|             | Buah Naga       | 10
|             | Jeruk           | 10
|             | Kelapa          | 10
|             | Nanas           | 10
|             | Pepaya          | 10
|             | Stroberi        | 10
Train         | Anggur          | 120
|             | Buah Naga       | 120
|             | Jeruk           | 120
|             | Kelapa          | 120
|             | Nanas           | 120
|             | Pepaya          | 120
|             | Stroberi        | 120
Validation    | Anggur          | 30
|             | Buah Naga       | 30
|             | Jeruk           | 30
|             | Kelapa          | 30
|             | Nanas           | 30
|             | Pepaya          | 30
|             | Stroberi        | 30

## Network
In this model, we design using the Convolutional Neural Network (CNN) architecture, besides that we also augment our dataset by enlarging the image, cropping the image, and resizing the image. This augmentation process is expected to further train the model to learn the dataset. After successfully classifying the images, we save the results of the tensorflow model that we have designed in the form of buah.h5. We also convert the model results to 6_Varians.tflite to simplify the process of making the application.

## Built With
* [Tensorflow Keras](https://www.tensrflow.org) - The AI framework used

## Authors
* **Ilyasa Affan Arinto - M2012F1316**
* **Sheerlyn Eliza Febriyana - M7012F1312** 
