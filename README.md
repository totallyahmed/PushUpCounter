# PushUpCounter
A simple program using Mediapipe and OpenCV to count the number of Push Ups done. The main goal is to ensure proper form while doing Push Ups so as to achieve maximum effect. 

The code above is from PoseModule.py and serves a few functions

Activate mediapipe’s Pose Detection module.
- Detect the human body.
- Finds the position of the different landmarks on the human body based on the model. (Landmarks are shown in image above).
- Finds the angle between joints (depending on which joints you select). For my Push Up program, I chose to find the angle at the elbow, shoulder, and hip as - those are vital for proper push-up form.

Next would be the code for the actual Push-up counting. In this, we will use the PoseModule and determine whether a push-up should be considered proper or improper form.

One important thing to note is from Line 17–21. Determine the resolution of your image captured from your camera, and from there adjust the pixel values when drawing the rectangles for the Push-up count, etc. (Lines 68–82).

![alt text](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*JJCbfzhTySIqKr1L5pDkpQ.png)
