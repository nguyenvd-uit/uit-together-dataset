# UIT-DroneFog

Author: *Minh T. Tran, Bao Tran, Nguyen D. Vo, Khang Nguyen*

Paper: *UIT-DroneFog: Toward High-performance Object Detection Via High-quality Aerial Foggy Dataset*

Organization: *UIT-Together*

Registering to use UIT-DroneFog: [[Link](https://forms.gle/4PpEspSKVeQtFjbbA)]

![](https://i.imgur.com/2H3pTCK.jpg)

Exemplary samples in UIT-DroneFog dataset.
## Foggy simulation process
In this work, the imgaug library was implemented to create synthetic fog for our dataset. We simulated fog on the UIT-Drone21 dataset with the use of this library’s Fog class, which has predefined different parameters. This class executes a single layer per image with a configuration leading to fairly dense fog with low-frequency patterns. However, to simulate suitable fog with the image’s size of the chosen dataset, we decided to adjust two parameters, which were alpha_min “0.75 and density_multiplier = 0.7, and kept other parameters as the default library (https://imgaug.readthedocs.io):

-	The alpha_min (default value of (0.7-0.9)) parameter indicates the minimum alpha value when blending fog noise with the image. The higher value leads to fog being "everywhere". 
-	The density_multiplier (default value of (0.4-0.9)) parameter is the Late multiplier for the alpha mask. Setting this higher to get denser fog wherever it is visible. 

## Dataset Description

UIT-DroneFog consists of 15,370 aerial images captured by drones with about 600,000 million bounding boxes of various means of transportation and pedestrians. There are four classes in this dataset: Pedestrian, Motor, Car, and Bus. Moreover, UIT-DroneFog has the distinguishing highlights:
* Variety of high-quality images: The foggy simulation process used images captured by high-end drones with 3 different resolutions (3840x2160, 1920x1080, 1440x1080), which led to our foggy images being all in high-quality images and are not blurred, distorted, skewed, or obscured. 
* Variety of context: Every image in our dataset is unique. They differ in fog distribution, capturing angle, and height. Moreover, we simulated fog not only in one place but in various places in different cities in Vietnam. 
* The challenge comes from data classes: Because this dataset was made on Vietnam streets, the vast majority of objects are motors. This data imbalance is a tough challenge for detectors to work efficiently. Besides, motors densely appear on the roads and they are very small, which leads to the difficulty in detecting these objects quickly. 

## Citation
If the project helps your research, please cite this paper.

```
@inproceedings{tran2021uit,
  title={UIT-DroneFog: Toward High-performance Object Detection Via High-quality Aerial Foggy Dataset},
  author={Tran, Minh T and Tran, Bao V and Vo, Nguyen D and Nguyen, Khang},
  booktitle={2021 8th NAFOSTED Conference on Information and Computer Science (NICS)},
  pages={290--295},
  year={2021},
  organization={IEEE}
}
```