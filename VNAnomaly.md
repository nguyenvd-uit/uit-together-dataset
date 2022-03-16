# VNAnomaly

Organization: *UIT-Together*
Registering to use Dataset: [[Link](https://forms.gle/Zdts8TcstLRAd1pZ9)]



The VNAnomaly dataset consists of 89 training videos and 96 evaluating videos that include real-world anomalies in Vietnamese street. The anomaly types contain 4 common human-related anomalies in the street of Vietnam including fighting, assault, vandalism, and robbery. Because the VNAnomaly is an unsupervised dataset, we will not explicitly define these anomaly types. The reason we choose the above anomaly types is the popularity of these types compared to other ones. In addition, these anomaly types are also relevant to the safety of public lives and assets in Vietnam’s urban environments. However, there are some unusual events that are not mentioned such as traffic accidents. Therefore, we will continue to provide more anomaly types soon.
Our dataset surpasses existing unsupervised datasets from
the following three aspects.

1. To the best of our knowledge, this is one of the first unsupervised datasets that capture the Vietnamese scene.
2. Larger data volume: VNAnomaly has 578,609 training frames and 75,214 evaluating frames, which is bigger than existing unsupervised benchmark datasets.
3. Higher scene diversity: Our dataset contains 36 scenes with different aspects such as different camera angles, times of the day. Furthermore, to ensure the context that the model learns in the training stage matches the testing phase, the scenes in the training set are required to be suitable with the testing set. As compared with ShanghaiTech dataset, number of scenes in our dataset triples them. 

To enhance the dataset’s quality, we constrain the context in this dataset to the street in Vietnam captured by the surveillance camera. We search videos on Youtube using text search queries in the Vietnamese language. In addition, to ensure the videos collected from Youtube are surveillance videos, we closely monitor the context in each video and only choose the videos that are not related to commercial purposes and are captured by surveillance cameras. After that, following the collecting process in [4], we get rid of the videos that do not satisfy the following conditions: manually edited, prank videos, not captured by CCTV cameras, taken from news, captured using a hand-held camera, and containing compilation. Additionally, we also try to collect training videos that have some similarities with the videos in the testing. The training sequences last seven and a half hours, whereas the testing sequences last approximately 1 hour with 110 anomalous events. In Figure 3, we show normal and abnormal frames with a nearly similar scene.




## Citation
If the project helps your research, please cite this paper.

```
@inproceedings{vu2021vnanomaly,
  title={VNAnomaly: A novel Vietnam surveillance video dataset for anomaly detection},
  author={Vu, Tu N and Dinh, Toan T and Vo, Nguyen D and Tran, Tung Minh and Nguyen, Khang},
  booktitle={2021 8th NAFOSTED Conference on Information and Computer Science (NICS)},
  pages={266--271},
  year={2021},
  organization={IEEE}
}
```

