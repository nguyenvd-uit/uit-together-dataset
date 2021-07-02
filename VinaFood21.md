# VinaFood21

Author: *Thuan Trong Nguyen, Thuan Q. Nguyen, Dung Vo, Vi Nguyen, Ngoc Ho, Nguyen D. Vo, Kiet Van Nguyen, Khang Nguyen*

Paper: *VinaFood21: A Novel Dataset for Evaluating Vietnamese Food Recognition, RIVF2021*

Organization: *UIT-Together*

Registering to use Dataset:  [[Link](https://forms.gle/1dKs2kVpJWT4473G9)]

![](https://i.imgur.com/gzqaTwi.png)
Illustration 21 dishes in VinaFood21


## Category Selection
Vietnamese cuisine encompasses diverse dishes from the mainstream culinary traditions in all three regions of Vietnam to the street food with original and creative recipes. We conduct a small survey on the Internet to choose the most favorite street food and dishes in typical traditional southern Vietnamese meals. Eventually, we statistics 21 dishes to continue to data collection for our dataset.

## Data Collection and Pre-processing
Most of the images were collected from social networking siteslike Instagram, Facebook, Bing, Flickr posted by users with relatedtags. We expanded search terms by adding keywords, such as foodand dish.

After this step, we collected more than 30,000 color images, withno size limit. These images are saved in21folders for each dish.However, these images may be kept in an incorrectly labeled folder.Furthermore, images are low quality, distorted, and duplicate. So wedo this by removing them and doing the labeling. The label set isassigned numbers 0-20.

## Label Validation
In this phase, we perform two different sub-stages to checkmistaken in data labeling. The two sub-stages are described as follows.‚
* Self-checking: Re-check your labels.‚
* Cross-checking: We cross-check each other’s labels. If we findany errors in the dataset, we will discuss each other.

## Dataset Description
After completing the above works, VinaFood21 contains 13,950 images are corresponding to 21 dishes. The total dataset size is 2GB.The number of images per category is in the range of (300,1200) .
VinaFood21 is a more comprehensive food dataset that surpasses existing Vietnamese Food datasets from the following three aspects.
1. Larger data volume: VinaFood21 has 13,950 images from21dishes, which has created a new milestone for complexVietnamese food recognition.
1. More extensive category coverage:It consists of21categories, which is about 2~3 times thatof existing Vietnamese food datasets.
1. Higher diversity: Foodcategories from our dataset cover various high intra-class distances(different look but similar type) and low inter-class distances (similarlook but different type), including both street food and a daily meal.Moreover, our dataset is more challenging in various layouts, sidedishes, and dishes in different lighting conditions

## Citation
If the project helps your research, please cite this paper.

```
@article{Thuan,
  title={VinaFood21: A Novel Dataset for Evaluating Vietnamese Food Recognition},
  author={Thuan Trong Nguyen, Thuan Q. Nguyen, Dung Vo, Vi Nguyen, Ngoc Ho, Nguyen D. Vo, Kiet Van Nguyen, Khang Nguyen},
  booktitle={In Proceedings of the 15th IEEE-RIVF International Conference on Computing and Communication Technologies (RIVF)},
  pages={},
  year={2021},
  organization={IEEE}
}

```
