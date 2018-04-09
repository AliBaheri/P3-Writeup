## **Behavioral Cloning** 

**Behavioral Cloning Project**

The goals / steps of this project are the following:
* Use the simulator to collect data of good driving behavior
* Build, a convolution neural network in Keras that predicts steering angles from images
* Train and validate the model with a training and validation set
* Test that the model successfully drives around track one without leaving the road
* Summarize the results with a written report

### My project includes the following files:
* model.py containing the script to create and train the model
* drive.py for driving the car in autonomous mode
* model.h5 containing a trained convolution neural network 
* writeup_report.md or writeup_report.pdf summarizing the results

### Overall hardware setup:

<p align="center">
<img width="500" src= "https://github.com/AliBaheri/P3-Writeup/blob/master/images/overal_hw.png">

### Overall software setup:

<p align="center">
<img width="600" src= "https://github.com/AliBaheri/P3-Writeup/blob/master/images/overal_sw.png">

### Data

During the training, the simulator captures data with a frequency of 10hz. In fact, at a given time step it recorded three images taken from left, center, and right cameras:

<p align="center">
<img width="800" src= "https://github.com/AliBaheri/P3-Writeup/blob/master/images/cameras.png">


### Model Architecture and Training Strategy

<p align="center">
<img width="350" src= "https://github.com/AliBaheri/P3-Writeup/blob/master/images/model.png">


<p align="center">
<img width="400" src= "https://github.com/AliBaheri/Vehicle_Detection_SDCND/blob/master/output_images/nonCar_HOG.png">


#### 2. Attempts to reduce overfitting in the model

The model contains dropout layers in order to reduce overfitting (model.py lines 21). 

The model was trained and validated on different data sets to ensure that the model was not overfitting (code line 10-16). The model was tested by running it through the simulator and ensuring that the vehicle could stay on the track.

<p align="center">
<img width="600" src= "https://github.com/AliBaheri/Vehicle_Detection_SDCND/blob/master/output_images/nonCar_HOG.png">


#### 3. Model parameter tuning

The model used an adam optimizer, so the learning rate was not tuned manually (model.py line 25).

<p align="center">
<img width="600" src= "https://github.com/AliBaheri/P3-Writeup/blob/master/images/sample_images.png">

