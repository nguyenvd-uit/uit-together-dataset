# UIT-TASTET21

Author: *Nguyen D. Vo, Vy Le, Phuc Nguyen, Tai Pham, Thang Truong, Kiet Huynh, Huyen Van, Dinh Minh, Ngoc Ho, Khang Nguyen*

Paper: *A Novel Dataset for Vietnamese New Year Food Classification*

Organization: *UIT-Together*

Registering to use Dataset: [[Link](https://forms.gle/FymxNLdN44oAjUjdA)]

![](https://i.imgur.com/EnGKnLs.jpg)

Illustration 15 dishes in UIT-TASTET21 dataset.


## Data collection
UIT-TASTET21 is a dataset on snack foods consumed during the traditional Tet holiday in Vietnam. This set contains color images of varying sizes, primarily the RGB color system. We have gathered it from various sources, the majority of which are social networks and websites that allow the use of photos. We choose the dishes (mostly candied fruits), based on their characteristics (traditional versus modern), foods types (cakes, candies, dried nuts, dried fruits,...), and various eating contexts (whether main courses, served with other dishes or for decorative purposes only). In particular, UIT-TASTET21 (Figure 3) includes 18 distinct types of snack foods (Candied Ginger, Candied Kumquat, Roasted watermelon seeds, Candied Kiwi, Pistachio, Sunflower seeds, Banh Chung,  Candied Soursop, Banh Tet, Almond, Cashew, Dried Peanut, Mung bean cake, Walnut,  Pumpkin seeds, Candied lotus seed, Dried peas, Dried soybeans).

## Data Refinement and Annotation
We've constructed a workflow to ensure that the data collected is appropriate for the research purpose. A lot of efforts have been put into manually eliminating images with inappropriate material or context, images that were unclear or too small in size, or shots where the target dish was too much obscured by other objects, such a time-consuming task. Images of the same food, however, packaged and decorated in different ways, are retained for the sake of data’s diversity. After obtaining the fine-tuned data, we proceeded to label at the image level (Figure 2).

Additionally, we enhance our dataset's quality by two two-stage validation. In the first stage, each annotator re-checks their label. In the second stage, all annotators cross-check the label of their partner. If they find the error, they will discuss it together to get the final label.




## Statistics and Data analysis
We present a dataset with 18 dishes typically found during the Vietnamese traditional Tet holiday. There are a total of 77,000 images divided into two definite sets with a ratio of 8:2. The training set consists of 63,840 images, whereas the test set has 14,041 images. The ratio of each food’s images in two subsets is randomly divided. Real-world data goes hand in hand with challenges; this means that the accuracy and performance of a deep learning model or machine learning model will be heavily influenced by the obstacle that the training data presents. By raising these concerns, we hope to lay the groundwork for optimal solutions proposed in the future.  
1. **Food images contain multiple confounding factors.** Dishes aren't always served separately (Figure 4 – Right) but instead put close to each other to enrich the meal. In addition, eating utensils (bowls, plates, glasses, etc.) and decorative items (lamps, vases, tablecloths, etc.) also contribute to visual noise in the images.
2. **Dishes come in various forms.**  Although the same type of dishes, they are prepared using different recipes, resulting in a wide range of shapes and colors (Figure 4 – Left). Traditional dishes with a lot of designs will appeal to consumers, so this is an element that appears very often on data images.
3. Several dishes with typical Vietnamese characteristics have relatively little data: Many delightful dishes are still unfamiliar with international friends, as are the facts on their data to which researchers have given little attention. Some foods have distinct flavors and a high commercial value (such as Banh in, Candied Ginger, Candied Kumquat, ...).
4. Several dishes in this data collection have a lot of similarities: This sameness makes them very confusing and challenging. However, even if both products are made from the same materials and undergo similar processing, the final product is noticeably different, reflecting Vietnam's distinct regional identities. 

## Citation
If the project helps your research, please cite this paper.

```


```
