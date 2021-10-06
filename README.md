<img src="https://user-images.githubusercontent.com/79296149/136213914-ecd296c7-0090-4785-8240-4fdb08089d7d.png" width="300px" height="300px">

# VirtualMouse
**#About**
Operating entire  mouse operation on screen using gesture

## Title
`Contactless Lifestyle`

## Description
We have created 1 modules
* `Virtual Cursor` (Module for using machines such as ATMs and vending machines)

These modules are both gesture controlled and does not require any physical contact. 


### Need for the project
According to current evidence, COVID-19 virus is primarily transmitted between people through respiratory droplets and contact routes. During this pandemic situation, it is advised to have less human contact as much as possible.
So we present an application of neural networks and image processing techniques to enable people to use gestures to operate the public machines that traditionally required physical contact.

<b>In the First module ' Virtual Cursor' user can control the entire screen by operation like click,move and double-click.This means without interacting with mouse or any external device he can control the screen.</b>

Algorithm for Cursor module

1. First we will capture the video and will pass the frames through our application. Our application will give the coordinates of the given 21 landmarks

2. Among all the 21 landmark we are extracting only the first finger landmark and using its co-ordinates(x and y)

3. We mapped the relationship between the displacement of the finger and the displacement of the cursor on the screen.

4. Once the mouse is synchronized then using different gestures for operations like click,move and double-click 


## Application

### Cursor 
1. It can be used to operate any device with camera instead of a keypad
2. The speed and accuracy of taking the input and recognizing gestures makes it a viable alternative to keypad operated devices.


## Tech Stack
Live video feed is acquired using the device camera itself. OpenCV (Open Source Computer Vision Library)  library is used for real-time computer vision.
You can use get(CAP_PROP_FPS) or get(CV_CAP_PROP_FPS) to get frames per second. 
A Video is made up of multiple still images known as Frames, 60 FPS means there are 60 images per second of video. All images are passed through Mediapipe.
Image Acquisition is done in real-time, and sent to mediapipe library(An open source google library) for the coordinates then passed through deep learning to get the Gesture.



## Libraries and dependencies required for the project (If any)
Hack uses python with opencv,mediapipe,numpy,pandas,keras

## Installation steps: A clear sequence of steps to run your hack
Download Python from : https://www.python.org/

Once python is installed run
`pip install requirements.txt`

<b> Running Cursor </b>
1. change directory to 'Cursor'
2. Run `Cursor.ipynb`

## Declaration of Previous Work
We had implemented the similar method for recognising the American sign language. In this project we have modified the application for Lift Module. And used the landmark acqusitions as same as before for the Cursor. However in the cursor we have added the stabelizing and mapping functions and added cursor control to it.



