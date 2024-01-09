# Geospatial Object Detection using Aerial Imagery

<p>
<a href="https://colab.research.google.com/drive/1whYgdDWQ3fcf8molrXSeAfqzeyh7x0wW">
<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a> </p>

## Introduction

<p align="justify">
Multi U-Net architecture has transformed aerial image object detection, pioneering advancements in geospatial analysis. This modified U-Net model excels in complex multi-class segmentation scenarios, leveraging spatial information effectively. The project employs a sophisticated image processing pipeline, maximizing deep learning model training through Min-Max scaling and Patchify techniques. It utilizes performance evaluation metrics like the Jaccard coefficient and a custom loss function hierarchy combining Focal Loss and Dice Loss for efficient model training. Results demonstrate Multi U-Net's ability to handle specific item types, reduce false positives/negatives, and adapt to diverse datasets and domains. Its improved segmentation precision benefits environmental monitoring, disaster management, and urban planning, showcasing its potential for impactful decision-making processes across various disciplines.
</p>


## Technical Stack

|<img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original.svg" alt="Python" width="100" height="100"/>&nbsp;|
<img src="https://github.com/devicons/devicon/blob/master/icons/jupyter/jupyter-original-wordmark.svg" alt="Jupyter" width="100" height="100"/>&nbsp;|
<img src="https://github.com/devicons/devicon/blob/master/icons/numpy/numpy-original-wordmark.svg" alt="Numpy" width="100" height="100"/>&nbsp;|
<img src="https://github.com/devicons/devicon/blob/master/icons/pandas/pandas-original-wordmark.svg" alt="Pandas" width="100" height="100"/>&nbsp;|
<img src="https://github.com/valohai/ml-logos/blob/master/matplotlib.svg" alt="MatplotLib" width="100" height="100"/>&nbsp;|
<img src="https://github.com/valohai/ml-logos/blob/master/keras-text.svg" alt="Keras" width="100" height="100"/>&nbsp;|
<img src="https://github.com/devicons/devicon/blob/master/icons/tensorflow/tensorflow-original.svg" alt="TensorFlow" width="100" height="100"/>&nbsp;|


## Dataset

<p align="justify">
<a href="https://humansintheloop.org/">Humans in the Loop</a> has published an open access dataset annotated for a joint project with the <a href="https://www.mbrsc.ae/">Mohammed Bin Rashid Space Center</a> in Dubai, the UAE. The dataset consists of aerial imagery of Dubai obtained by MBRSC satellites and annotated with pixel-wise semantic segmentation in 6 classes.
</p>

### Semantic Annotation

The dataset includes 72 images grouped into 8 larger tiles.
The images are labeled and contain the following classes:

| Name       | R   | G   | B   | Color                                                                                              |
| ---------- | --- | --- | --- | -------------------------------------------------------------------------------------------------- |
| Building   | 60  | 16  | 152 | <p align="center"><img width = "30" height= "20" src="./Content/label_building.png" /></p>   |
| Land       | 132 | 41  | 246 | <p align="center"><img width = "30" height= "20" src="./Content/label_land.png" /></p>       |
| Road       | 110 | 193 | 228 | <p align="center"><img width = "30" height= "20" src="./Content/label_road.png" /></p>       |
| Vegetation | 254 | 221 | 58  | <p align="center"><img width = "30" height= "20" src="./Content/label_vegetation.png" /></p> |
| Water      | 226 | 169 | 41  | <p align="center"><img width = "30" height= "20" src="./Content/label_water.png" /></p>      |
| Unlabeled  | 155 | 155 | 155 | <p align="center"><img width = "30" height= "20" src="./Content/label_unlabeled.png" /></p>  |


<p>The trained models can be found <a href="https://drive.google.com/drive/folders/16IpkE45L2x0zmlykJXDDApmhDL14eFa-?usp=sharing">here.</a></p>


### Results

Predictions on Validation Set Images:

<p align="center"><img width = "95%" height= "auto" src="./Content/prediction_1.jpg" /></p>
<p align="center"><img width = "95%" height= "auto" src="./Content/prediction_2.jpg" /></p>
<p align="center"><img width = "95%" height= "auto" src="./Content/prediction_3.jpg" /></p>
<p align="center"><img width = "95%" height= "auto" src="./Content/prediction_4.jpg" /></p>


