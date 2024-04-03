# Bone-Fracture-Classification-and-Detection

This project has for goal to compare the methods used, in the literature, to classify radiography images presenting bones in order to detect a potential condition (mainly fractures).

## Models
The most popular methods used for this type of problem are CNNs able to recognize patterns in an image, thus allowing and easy recognition of a potential condition. 
The CNNs tested here are DenseNet-201 and Inception-ResNet-v2. Both of these models have been trained on the same dataset, MURA.

## Dataset
For this project, radiographies of bones, healthy and abnormal were needed to be able to train the models and classify them. In the litterature, the MURA dataset seemed to be well used.  
This dataset was created by Stanford University for a classification contest. It regroups more than 40 000 radiographies from 14665 studies split into a training and a validation set. 
The test set of the contest was not available as of the time this project was impemented so the training and validation set were merged, in a first time, and split in three sets: training (80%) validation (10%) and test (10%)

## Method
The same method was used on both the models presented in order to compare their respective performances : learning rate =  1e-5, epochs = 10, loss = binary crossentropy
The experiment was conducet three times wit a different number of images (100,3000 and 10000 images) to see the impact of the number of data.
Sadly, the experiment using the whole dataset wasn't possible because of the limitations of the machine used for the training. 

## Results

### 100 images
Here are the graphs obtained during the training:


[![Densenet201Training](results-100
/densenet_training_results.png)](https://github.com/kevinbecquet/Bone-Fracture-Classification-and-Detection/blob/main/results-100)


### 3000 images 


### 10 000 images
 
