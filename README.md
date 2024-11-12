# Perfect Pull Ups 

## Description
The goal of this project is to estimate if a pull-up, taken from video, is a full range-of-motion, or "perfect," pull-up. This project utilizes a pre-trained deep learning human pose estimation model to extract key points and assess the form of the pull-ups exercise. 

By analyzing the spatial relationships between these key points, using vector arithmetic and trigonometry, the program calculates the angle of arm extension and flexion. To ascertain the completeness of the pull-up movement, the program compares the calculated arm extension or flexion angle against a predefined threshold indicative of full extension or flexion. A "perfect" pull-up is completed when the subject is in the bottom state in full-extension, moves to the top state at the predefined threshold for flexion, then back to the bottom state in full-extension.

The pre-trained deep learning model used in this project is a variant of **Caffe** model.

The layers output feature maps that correspond to keypoints during the human pose estimation task.
Example heatmap of all of the 18 keypoints from the model:
<img src="media/heatmaps.png" alt="Screenshot" width="1180"/>

## Visuals
This is the output of the program, given an input of a video of a me doing pull-ups. You can see that when I do partial reps (not full range-of-motion) it will not increment the rep:

<img src="media/cam_test.mp4" alt="Pullup test" width="400"/>

## Installation
- OpenCV
- Numpy
- Enum

## Author
- [Cameron Boydd](https://github.com/camboydd)
