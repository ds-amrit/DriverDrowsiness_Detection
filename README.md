# DriverDrowsiness_Detection
Real-time analysis of driver's state: active, drowsy or sleeping.

## What is Driver Drowsiness ? 

We have heard of many accidents that involve drivers lacking focus. Most cases are due to sleep factor (drowsiness).

Psychological studies have demonstrated that drowsiness can significantly impair productivity and the quality of work outcomes. For example, drowsy driving, usually caused by sleep loss, nights or very long working hours, is reported as one of the main causes of serious accidents.


## Objective:

* To reduce the road accidents due to driver fatigue.

* To detect driver’s state (Active, Drowsy, Sleeping) in real time by tracking its eye movement.

* Alert the driver as its state changes from drowsy to sleeping.

## Block Diagram:

![image](https://user-images.githubusercontent.com/107737679/229684325-b0b3933c-e581-404f-91a0-fa374f629348.png)

## Proposed System:

A webcam based system is used to  detect driver’s fatigue from the face image  using image processing and machine learning techniques.
Two main python modules used are:
OpenCV: Is a open source library that allows you to perform image processing and computer vision tasks.
Dlib: is a open source Landmark facial detector with pre-trained models to detect semi rigid objects in addition to human faces.

## So how does DLib detects my face ? 

Dlib is used to estimate the location of 68 coordinates (x,y) that map the facial points on a person’s face like the image below:
![image](https://user-images.githubusercontent.com/107737679/229684647-0041cc7d-8e5c-4d23-8a33-79dae51fe77a.png)
Important Landmark points for different features:
 Parts
Points
*Left Eye
[36-41]
*Right Eye
[42-47]
Nose
[27-35]
Mouth 
[48-67]



To run this app you need to download the shape_predictor_68_face_landmarks.dat file from the link below:
https://www.kaggle.com/datasets/sergiovirahonda/shape-predictor-68-face-landmarksdat

