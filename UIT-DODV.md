# UIT-DODV

Author: *Linh Truong Dieu, Thuan Trong Nguyen, Nguyen D. Vo, Tam V. Nguyen, Khang Nguyen*

Paper: *Parsing Digitized Vietnamese Paper Documents*

Organization: *UIT-Together*

Registering to use Dataset: [[Link](https://forms.gle/wCiv9LgKdnjtTCUh6)]

![](https://i.imgur.com/9R58GiZ.png)
Exemplary samples in UIT-DODV dataset.

## Data Collection
We collected the data from the scientific paper available on the website of Can Tho University (CTU). In addition, we used the physical scanner and the scanning app on smartphone to scan the hard-copy of National Conference "Some Selected Issues of Information Technology and Communication" from the following versions:

* The XXI edition with the topic "Internet of Things" was held from July 27-28, 2018, at Hong Duc University, Thanh Hoa Province.
*  The XXII edition with the topic "Transforming the number of socio-economic operating in the Industry 4.0" was held from June 28 to 29, 2019, at Thai Binh University, Thai Binh Province.


The images in UIT-DODV are created by converting paper documents to digital images, using document conversion program, physical scanners and scanning app on smartphone. The purpose of collecting data from multiple sources is to create diversity for data in terms of layout, presentation form and data domain is also expanded with scanned images instead of just using the transferred image convert from PDF. After collecting the desired data, we proceeded to label attachments. Instead of tagging the data from where, we used the pretrain model from the PAA method to predict the bounding box for the object before manually editing those objects.


## Category Selection
We followed other image-based document datasets to select the categories. In particular, the first selected object is **Table** - appearing in most published datasets. **Figure** is the simplest and most effective way to turn complex ideas into a concise form, which can be a statistical graph that helps visualize the results of research. Shapes include natural sceneries, graphs, charts, layout designs, block diagrams, or maps. Likewise, **Formula** is equally important to describe relationships between concepts and objects concretely and efficiently. The formulas are usually numbered and may occupy several text lines. In addition, the formula object that contains equations and non-math text in a math region leads to the challenge of this object. Besides, with the desire to build a dataset that can be used for many different tasks such as OCR or VQA, we chose to add a new label, **Caption** - presenting a brief and yet complete explanation of the figure or table. The caption for a figure usually appears below the graphic; for a table, above.

## Dataset Description
UIT-DODV is the first Vietnamese document image dataset, including 2,394 images with four classes: Table, Figure, Caption, Formula.  UIT-DODV converted 1,696 images from PDF with size 1,654 x 2,338, 247 images scanned from the physical scanner and expanded with 451 images scanned from the smartphone.
    
UIT-DODV has the following highlights: 

1. Variety of images: images in our dataset are of two types, with images converted from PDF as complete documents and images. Scan images often have lower resolutions depending on the scanning angle as well as the lighting conditions that can cause the document page to be blurred, distorted, skewed, or obscured. 
2. Variety of layout: data collected from other scientific conferences/journals, a common feature of these conferences/journals is that they often use their templates (typically document pages can represent document pages in the form of one column or two columns). 
3. The challenge comes from data classes: with the simultaneous use of two formula objects (Formula) and Caption creates a challenge for our dataset as well. As in building detection models for these objects. The vast majority of a document page is represented as text, so spotting these objects quickly is very difficult.

## Annotation Formats
The annotation files follows 3 format: 
* [COCO](http://cocodataset.org/#format-data)
*  [Pascal VOC](https://pjreddie.com/media/files/VOC2012_doc.pdf)
* [YOLO](https://github.com/AlexeyAB/darknet)
## Citation
If the project helps your research, please cite this paper.

```
@article{Linh,
  title={UIT-DODV: Parsing Digitized Vietnamese Paper Documents},
  author={Linh Truong Dieu, Thuan Trong Nguyen, Nguyen D. Vo, Tam V. Nguyen, Khang Nguyen},
  booktitle={In Proceedings of the The 19th International Conference on Computer Analysis of Images and Patterns (CAIP)},
  pages={},
  year={2021},
  organization={Springer}
}

```
