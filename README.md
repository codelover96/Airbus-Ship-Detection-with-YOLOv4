# Airbus-Ship-Detection-with-YOLOv4
Airbus Ship Detection challenge with YOLOv4 object detector
Back in 2019 Airbus published a challenge for ship detectio on Kaggle. Airbus provided a large dataset of satellite ship images from SPOT satellite.
There are many attempts on solving this challenge, published on Github. In this attempt I'm using YOLOv4 object detector. Other have used Mask R-CNN, Single Shot Detector etc. This challenge is very popular across the Deep Learning community and AI researchers. Sometimes this dataset is used as a performance metric and evaluation of new Deep Learning models.

#### Why YOLOv4
Altough YOLOv4 does not perform well when there are objects really close to each other which is the case for many images on this dataset, it is considered to be really fast. I chose to use yolo simply because of my familiarity with it in the past. In the future I plan on solving this problem with Mask R-CNN.

#### More on the Dataset
[Airbus Ship Detection Challenge on Kaggle](https://www.kaggle.com/c/airbus-ship-detection)

* Dataset consists of more than 100k images of 768x768 pixels.
* Has a size of 28.9 Gb compressed and close to 31 Gb uncompressed
* Contains a test and train subset

#### Useful Links
[Airbus Ship Detection - Traditional v.s. Convolutional Neural Network Approach](http://cs229.stanford.edu/proj2018/report/58.pdf) by Ying Chen, Junwen Zheng, Zhengqing Zhou 

~codelover96
