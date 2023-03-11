# LEVIR-CD

LEVIR-CD is a new large-scale remote sensing binary change detection dataset, which would help develop novel deep learning-based algorithms for remote sensing image change detection.

## News

- 20230311: We have supplemented geospatial information (e.g., latitude and longitude coordinates) for each sample in LEVIR_CD. Files and more information can be found [here](https://github.com/justchenhao/STANet/tree/master/LEVIR_CD_spatial_info). 

- 2021: we have provide more samples, namely [LEVIR-CD+](https://github.com/S2Looking/Dataset/tree/main/LEVIR-CD%2B/LEVIR-CD%2B).
-  
- 2020: first version of LEVIR-CD has released!

## Overview of LEVIR-CD

LEVIR-CD is a new large-scale remote sensing building Change Detection dataset. The introduced dataset would be a new benchmark for evaluating change detection (CD) algorithms, especially those based on deep learning.

LEVIR-CD consists of 637 very high-resolution (VHR, 0.5m/pixel) Google Earth (GE) image patch pairs with a size of 1024 × 1024 pixels. These bitemporal images with time span of 5 to 14 years have significant land-use changes, especially the construction growth. LEVIR-CD covers various types of buildings, such as villa residences, tall apartments, small garages and large warehouses. Here, we focus on building-related changes, including the building growth (the change from soil/grass/hardened ground or building under construction  to new build-up regions) and the building decline. These bitemporal images are annotated by remote sensing image interpretation experts using binary labels (1 for change and 0 for unchanged). Each sample in our dataset is annotated by one annotator and then double-checked by another to produce high-quality annotations. The fully annotated LEVIR-CD contains a total of 31,333 individual change building instances.

## Geospatial Distribution of LEVIR-CD

The bitemporal images in LEVIR-CD are from 20 different regions that sit in several cities in Texas of the US, including Austin, Lakeway, Bee Cave, Buda, Kyle, Manor, Pflugervilletx, Dripping Springs, etc. The Figure below illustrates the geospatial distribution of our new dataset and an enlarged image patch. The captured time of our image data varies from 2002 to 2018. Images in different regions may be taken at different times. We want to introduce variations due to seasonal changes and illumination changes into our new dataset, which could help develop effective methods that can mitigate the impact of irrelevant changes on real changes.

![samples](\assets\images\location.jpg)

## Examples of annotated samples

### Samples size of 1024 × 1024

![samples](\assets\images\samples.jpg)

### Cropped samples size of 256 × 256

 ![cropped_examples](\assets\images\crop_samples.jpg)

## Usage

The use of the images from Google Earth must respect the [Google Earth terms of use](https://www.google.com/permissions/geoguidelines/). All images and annotations in LEVIR-CD can only be used for academic purposes, but are prohibited for any commercial use.

## About

We are from LEVIR, which is the abbreviation of ours’ laboratory: LEarning, VIsion and Remote sensing laboratory. Visit the lab [homepage](http://levir.buaa.edu.cn/) for more details.

If you have any the problem or feedback in using LEVIR-CD, please contact

- Hao Chen at justchenhao@buaa.edu.cn
- Zhenwei Shi at shizhenwei@buaa.edu.cn

## Cite

If you use this dataset for your research, please cite our papers.

```latex
@Article{Chen2020,
AUTHOR = {Chen, Hao and Shi, Zhenwei},
TITLE = {A Spatial-Temporal Attention-Based Method and a New Dataset for Remote Sensing Image Change Detection},
JOURNAL = {Remote Sensing},
VOLUME = {12},
YEAR = {2020},
NUMBER = {10},
ARTICLE-NUMBER = {1662},
URL = {https://www.mdpi.com/2072-4292/12/10/1662},
ISSN = {2072-4292},
DOI = {10.3390/rs12101662}
}
```

You can also find the related code resources (STANet) [here](https://github.com/justchenhao/STANet) in GitHub.

