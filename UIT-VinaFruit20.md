# UIT-VinaFruit20

Author: *Thuan Trong Nguyen, Hai Le, Truong Nguyen,  Thinh Le,  Khanh Duong,  Quyen Tran,  Vu Bui, Hop Nguyen, Nguyen D. Vo, Khang Nguyen*

Paper: *An Empirical Evaluation Of Feature Extraction For Vietnamese Fruit Classification*

Organization: *UIT-Together*

Registering to use Dataset: [[Link](https://forms.gle/c7GCU4igG53PhVWp7)]

![](https://i.imgur.com/iUkFPHP.png)

Illustration 20 fruits in UIT-VinaFruit20


## Category Selection
Located in the tropical zone, Vietnam is truly a heaven when it comes to fruits. There are even tours arranged exclusively for tourists who love visiting orchards to witness how the fruits are grown and try fresh fruits in the garden. Many Fruit Festivals are held in many local annual, attracting millions of locals and foreign visitors. Therefore, we examined many websites about travels with several blogs written for Vietnamese cuisine then summarized the most well-known Vietnamese fruit, which received high recommendations from locals and foreigners. After that, we found that 20 popular fruits to start our first step to building the Vietnamese fruit dataset is to collect the data.

## 3.2.	Data Annotation
We primarily collect images from Google images. We expanded search terms by adding some keywords. In addition, we also used smartphones to take photos of fruit that we met on a daily day.  We collected approximately 100,000 images, which are saved in 20 different folders named by each fruit. However, these images may be kept in an incorrectly labeled folder. Furthermore, images are low quality and duplicates. Hence, we conduct data cleaning by removing duplicated and low-quality images as well as moving images to the correct folder. 
In the next step, we want to ensure neither mistakes in each class nor enhance our dataset's quality. Therefore, we performed two sub-stages to verify labels. 
* The first sub-stage is for each people re-check their label.
* The second is cross-checking each other's labels. If we find any errors in the dataset, we will discuss each other.



## Dataset Description
UIT-VinaFruit20 contains 63,541 images are corresponding to 20 Vietnam popular fruits, with the average images per class are about 3,700 images. UIT-VinaFruit20 is the first Vietnamese fruit dataset with four main features promising more challenges.  
1. **Diversity in the color of one fruit.** We collected both images from unripe fruit to the fruit we can eat, which has a different color in each period of fruit. Furthermore, the similarity in color between fruit is also an element concerned.
2. **Similar in shape.**  Fruit categories from our dataset cover various high intra-class distances (different look but similar type) and low inter-class distances (similar look but another type).
3. **Diversity in the appearance of fruit in the image.** We didn't limit the images to only contain one fruit in them. Therefore, the fruit can appear in various locations of an image with many sub-objects. For example, fruit can occur in a meal that includes others food, or fruit is set up into a basket gift contains another item.

## Citation
If the project helps your research, please cite this paper.

```


```
