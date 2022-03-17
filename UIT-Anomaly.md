# UIT-Anomaly


Author: *Dung Vo, Tung Minh Tran, Nguyen D. Vo and Khang Nguyen*

Paper: *UIT-Anomaly: A Modern Vietnamese Video Dataset for Anomaly Detection, NICS2021*

Organization: *UIT-Together*

Registering to use UIT-Anomaly: [[Link](https://forms.gle/uWaVkwF71AZcaaYG8)]

![](https://i.imgur.com/MsmPVCr.png)

Some samples of six anomalous activities in UIT-Anomaly dataset.
## Selecting Anomaly Categories
As far as we know, it is difficult to completely define anomalous behavior because there are a lot of aspects and different presentations in the realword, we clearly describe anomalous activities to minimize the ambiguity in creating fundamental truth. To mitigate the above issues, we consider the six following anomaly classes: Stealing, Traffic Accident, Fighting, Unsporting Behavior, and Against. We are interested in these anomalies because they have distinct features in Vietnam.


## Video Collection

We collect videos from Youtube by using keywords like “street violence”, “street stealing”, “marital combat”, “dog thief” and other words that have a similar meaning with each type of anomaly. With the normal behavior, we search for “security camera at school”, “CCTV at street”, “CCTV at home”, etc. Anomalous behavior in Vietnam is not captured by CCTV much, so we also collect other videos captured by smartphones, car black boxes. However, the number of videos captured by CCTV still accounts for the majority and is completely shot from real events.

## Video Cleaning
As a rule of the original regulation, we only use videos that they have not manually edited, so our annotator team checks each video to make sure. The number of videos that satisfy the regulation is not enough to decide to keep the original videos or the edited videos but they are still intact. After that, we re-edit videos by deleting borders, changing video speed to normal, etc., intending to make the video as close to the original as possible. Furthermore, we also remove videos with excessive modifications or videos with unclear anomalies.

## Video Annotation
Our dataset is annotated based on the weakly supervised approach so the training set just needs annotating at video-level. In addition, frame-level of the testing set is also annotated to evaluate the performance of the methods on the testing phase, that is, to confirm the start and end frames of anomalous activities. The dataset is finally accomplished after intense efforts over several months.

## Dataset Statistics
The UIT-Anomaly dataset includes a total of 224 muted videos captured at a frame rate of 30 fps with various resolutions. It has 104 normal and 120 anomalous videos. The total duration is more than 200 minutes, corresponding to 392,188 frames. We divide these videos into two subsets: the training set included 90 abnormal and 90 normal videos, while the test set consisted of the remaining 30 abnormal and the remaining 14 normal videos. Both training and test sets contain six classes of anomalies. UIT-Anomaly has the following highlights:

* Data size: Compared to other datasets for the anomaly detection problem, UIT-Anomaly can be considered as a sizable dataset with a total duration of more than 200 minutes, containing 314,843 training frames and 77,345 testing frames.
* Vietnamese context: UIT-Anomaly is the first dataset containing many typical Vietnamese contexts. Most of the benchmark datasets currently available were shot in China (CHUK Avenue, UCSD Ped 1, UCSD Ped 2, ShanghaiTech) or from Western countries (Subway dataset, UMN) or other countries (UCF-Crime).
* Variety of backgrounds: UIT-Anomaly is not only diversified in terms of the number of unusual types, but also in terms of the range of contexts, with 18 scenes including the road, the private home, the parking area, and more in a variety of weather, lighting, and camera angles. This makes our dataset more realistic, but it also brings obstacles when tackling the problem of anomaly detection in complicated contexts.

## Citation
If the project helps your research, please cite this paper.

```
@inproceedings{vo2021uit,
  title={UIT-Anomaly: A Modern Vietnamese Video Dataset for Anomaly Detection},
  author={Vo, Dung TT and Tran, Tung Minh and Vo, Nguyen D and Nguyen, Khang},
  booktitle={2021 8th NAFOSTED Conference on Information and Computer Science (NICS)},
  pages={352--357},
  year={2021},
  organization={IEEE}
}
```

