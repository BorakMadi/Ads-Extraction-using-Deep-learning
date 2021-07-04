# Ads-Extraction-using-Deep-learning

## Dataset
New dataset of advertisement images called AD dataset. It includes about six thousand RGB-images where each image contains at least one quadrilateral advertisement. The AD dataset includes a wide range of advertisements types and sizes, starting from billboards on the highway to advertisements in malls.

<img src="https://github.com/BorakMadi/Ads-Extraction-using-Deep-learning/blob/main/img_00096.png" width=25% height=25%><img src="https://github.com/BorakMadi/Ads-Extraction-using-Deep-learning/blob/main/img_00067.png" width=25% height=25%>

### Collecting and labeling images
The images of the AD dataset were collected automatically from the internet and labeled manually. We collected images that include advertisement using a python script called [Google images download](https://github.com/hardikvasa/google-images-download) which downloads images from google using given keywords. The resolution of the images varies from 256x144 to 2048x1080. The advertisements within these image have diverse perspective views.

We label the images using [Labelbox](https://labelbox.com/), the annotators went over each of the downloaded images and traced the boundary of each advertisement in the image. We define the boundary of an advertisement by its vertices in a counter-clockwise(CCW) order. In addition, we generate a binary mask using the annotated polygon for each image, where the pixels of the advertisement are marked by 1 and the background by 0. Hence, we have two types of labels for each image.

The dataset link : [AD Dataset](https://drive.google.com/drive/folders/1aTfES9zgNrIZhWnJVpNI779z8mWgtGkp?usp=sharing)

