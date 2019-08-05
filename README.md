# Blink_Detector

Blink Detector can be used to check the liveness of the video. Liveness of the video implies checking if the video is real or not.

In this project, we capture a video of 10 seconds. With that video, we check the number of blinks. We can add the threshold number of blinks to check the liveness you want. This code can also be used for live video with few changes in the code.

This project can be divided into sub parts. In the first part we capture the video of 10 seconds and save it as mp4 file. from there we use Opencv and dlib libraries to perform facial landmark detection and detecting the blinks. Each eye is represented by 6 (x,y) coordinates, starting at left corner of the eye and then working clockwise around the remaining region of eye. Eye Aspect Ratio(EAR) is the relation between these coordinates. The ratio can be defined as distance between vertical eye landmarks to the distance between horizontal eye landmarks. This ratio reduces rapidly when a person is blinking. 

Libraries Required: OpenCV, dlib   
Language Used: Python   
