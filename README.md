# Melanoma-Detection

Introduction - Skin Lesions Analysis

This is a Deep Learning project implemented using Neural Networks in Python programming language. 

Neural Networks is one of the many algorithmic leanring technique which is widely used in the Computer Vison domain. It is one of the many powerful Machine Learning model which provides you ways to tune a training model with hyper parameters such optimizers, leanring rate, regularizers etc that could considerably improve the metrics of the predictive model. 

Now, one of the biggest challege with Computer Vision Deep Learning projects is to find a platform with high computing capabilities. In this project, I have used the GPUs on Google Collab Pro with high-speed RAM at various stages. 

This project is divided into 4 stages. There can be multiple approaches, for starters,  this is one which I hvae implemented as a beginner.

Data:
Here, we are using dermascopic images of Skin Lesions. They high resolution pigmented images source from https://challenge2018.isic-archive.com/. There are a total of 10015 images that belong to 7 different melanoma types. 

Step 1 : Exploratory Data Analysis
The first step of analysing data is to understand what features represent the information at hand and how they vary within the data. This essentially means , in a classification problem, how many classes do we have and in what proportions do they exist. This data is highly skewed, i.e. we have proportionately more number of images for a specific melanoma type as comared to the other six classes. 

Step 2 : Data Preprocessing
For this analysis we are focused specifically on Disease Classification. That is to say that we want to identify which of the 7 melanoma types does the skin lesion fall under. There are three parts to Data Preprocessing :
  2.1 Converting images to numeric arrays / tensors and scale them to have values between 0 and 1 in floating point data type.
  2.2 Data Augmentation for treating Class Imalance
  2.3 Splitting the Data to Train : Val : Test :: 75:15:10

Step 3 : Building Models
Professor Alizadeh in class introduced the concept of Neural Networks like a form of art. You can play around with the architecture of the model and learn how they impact the learning of patterns in data. I started by building a simple Convolutional Neural Network with 6 Conv2D and Maxpooling2D layers this gave a test accuracy of 70%. Later I used MobileNet pretrained model and added a custome Activation Layer which gave a test accuracy of 82 % on data generated using Data Augmentation (class - balanced data).

Step 4 : Model Evaluation
Using a pretrained model certainly gave better with the CNN exposed to images of all classes proportionately while training.

Prediction & Conclusion-
Although 80% test acccuracy would not qualify to be an effective model for medical diagnosis. With more comupting capabilities and exploring more powerful Deep Learning techniques, various models can be used in combination that can prove to show great results with better predictive capabilities. 

This is a beginner's approach to a Computer Vision project of image classificaiton. Codes and details can be viewed in the Jupyter Notebook fines and presentation shared in this repository. Please feel free to leave a comment , I would love to get a feedback. 
