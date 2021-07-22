# UIT-Drone21


Registering to use Dataset: [[Link](https://forms.gle/nKbtYJqH6ZrpHrAu6)]

![](https://i.imgur.com/59eZj4I.png)
Exemplary samples in UIT-Drone21 dataset.

## Data Collection
Thanks to the advantage of high mobility, Unmanned Aerial Vehicles (UAVs) are used to provide many essential tasks in computer vision, bringing more efficiency and convenience than fixed surveillance cameras or ground moving sensors with limited angle and visibility. UAVs have many practical applications. For example, UAVs are used in the military to detect and locate enemies, patrolling the border. Furthermore, it can be used for anomaly detection, such as notice running in the forest and become criminals tracking devices for police. When ordinary cameras show a significant limitation, the UAV offers flexibility (moving under challenging terrains, operating independently, or being controlled remotely by the center or controller), wide field of vision. However, drone datasets are still limited, and they focus only on a few specific tasks, such as visual tracking or object detection in certain situations.

We built a novel dataset to advance drone-based image analysis tasks with complex scenarios that promise new challenges in this project. UIT-Drone21 was chosen from 23 short videos of approximately 13,066 fully labeled frames with bounding boxes for many tasks such as object detection, sing-object tracking, and multiple object tracking. We added approximately 2,304 frames (about 15,370 frames total) for object detection tasks. 



## Data Preprocessing
We have annotated approximately 15,370 frames from 23 videos and 2,304 frames of roughly 0.6 million bounding boxes across vehicles and road users in our dataset. We labeled four popular traffic participants, which included pedestrian, motor, car, bus. However, the characteristics of road traffic in Vietnam are very complex, and especially the motor took the majority. Therefore the motor took account most in the UIT-Drone21 dataset. In some areas in the image, the vehicles are too small to analyze their movements or perform classification on we will ignore.

## Dataset Description
UIT-Drone21 includes 23 videos of approximately 13,066 frames for object detection, single-object tracking, and multiple object tracking (DET, SOT, MOT) tasks. In addition, 2,304 frames for the object detection task. Drones took the videos and images at various urban locations (e.g., downtown streets, highways, intersections, junctions, roundabouts). UAVs shot videos during the day with two types of altitudes, high and low (low is from 20-40m, high is over 40m). Videos are recorded at 30 frames per second (30 FPS) with different resolutions (1920x1080, 1440x1080, 3840x2160 pixels). We conducted detailed quantitative research using the most recent state-of-the-art (SOTA) algorithms for each task. The experimental results have shown that the SOTA methods perform relatively poorly on our dataset due to new challenges emerging in drone-based natural scenes, e.g., high altitude, small objects, and camera movement. The challenge mainly focused on two tasks:
![](https://i.imgur.com/7Oeo91x.png)
Illustration annotated images in UIT-Drone21 dataset.
* **Task 1 - Object Detection.** UIT-Drone21 included a set of predefined classes (pedestrian, motor, car, bus). The task focus on detecting object from individual images taken from UAVs. We have divided the dataset into three parts. Specifically, the training set with 8,580 images, the validation set included 1,061 images, and the testing set contained 5,729 images.
* **Task 2 - Object Tracking.** In this task, we concentrate on tracking single objects or tracking multiple objects on video. The input of the object tracking problem is video frames. The system would conduct object detection, which is performed through object classification. After that, track and predict object movement. Due to high traffic density, the bounding box can be hidden by another, and the small object is one of the most challenging of this dataset. We have divided the dataset into two parts: training set (15 videos) and testing set (8 videos).


## Citation
If the project helps your research, please cite this paper.

```
@article{,

}

```
