# UIT-CVID21

Organization: *UIT-Together*

Author: *Truc Trinh, Nguyen D. Vo and Khang Nguyen*

Paper: *Phân loại phương tiện giao thông Việt Nam trong không ảnh, JSTIC*

Organization: *UIT-Together*

Registering to use UIT-CVID21: [[Link](https://forms.gle/aajmoJ7n9L6Hpsrk8)]

![](https://i.imgur.com/WCTHZQQ.png)

Illustration some samples in UIT-CVID21 dataset


## Category Selection
Economic growing makes the demand for transportation to be increasing that also leads to the growing number of means of transportation. This fact puts a lot of pressure on traffic management agencies with problems such as traffic congestion, traffic accidents, vehicle statistics and urban transportation planning; therefore, timely and stable solutions are needed. A large number of CCTV, radar sensors are installed to monitor vehicles and collect traffic information, which helps agencies to keep track of traffic flow, vehicle density and parking status. However, these methods do not provide a sufficient overview to develop and solve the current situations.

Recently, images taken from UAVs have been easy to collect and extreme useful due to their ability of covering large areas in a single image and high resolution in a small number of locations. Thanks to this high resolution, vehicles can be detected even small objects such as cars and motors. But, to be able to solve the problem of vehicle detection well, we have to have a good classification model which can deal with the current situation of traffic in Vietnam. So that, our team built a dataset named UIT-CVID21 (Classifying Vehicle In Image From Drone) which can reflect the reality of Vietnam traffic to create premises for later studies and address problems such as traffic density management, traffic separation and traffic congestion. UIT-CVID21 has 10,000 images which include four classes: bus, car, truck and van.
The reason for choosing these four classes is that during observation, we realize objects collected by drone from a height of over than 100m is quite small and may lead to confusion in the vision. In particular, confusion is more likely to occur in these two object pairs: bus – truck and car – van.


## Data Collection
After recording videos by drone, we choose 3,982 images with the resolution about 960 × 720 pixels which have a standard quality. The collected data have seen a change in the illumination and weather (daytime, cloudy, sunny and foggy) and the quite density flow of traffics: after selecting and annotating manually, we got about 50 bboxes, for a image. We believe that UIT-CVID21 is one of first dataset in the present time that can record the most diverse angles and clearly show the characteristics of Vietnamese road thanks to the flexibility of unmanned aerial equipment. Previous datasets are mostly shot by cameras with a fixed angle and constant height which the challenge is more different to datasets captured by drone like our UIT-CVID21.

## Data Preprocessing

After labeling in Pascal VOC format, we crop the image into small pieces of objects, then choose 10,000 sample and put them into four classes: bus, car, truck, van. Next, images are divided randomly into two parts train set and test set with the ratio 7:3 

## Dataset description
- 7,706 sample used for training:
    - Bus: 449
    - Car: 5,166
    - Truck: 1,281
    - Van: 810
- 2,294 sample used for testing:
    - Bus: 553
    - Car: 1,018
    - Truck: 314
    - Van: 406

## Citation
If the project helps your research, please cite this paper.

```
@article{cvid21@truc,
  title={Phân loại phương tiện giao thông Việt Nam trong không ảnh},
  author={Trịnh Thị Thanh Trúc, Võ Duy Nguyên, Khang Nguyễn},
  booktitle={Journal of Science and Technology on Information and Communications (JSITC)},
  pages={},
  year={2021}
}

```

