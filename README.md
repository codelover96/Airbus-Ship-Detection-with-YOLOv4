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
* Includes 2 csv files one containing the image name and the encoded pixels in Run Length Encoding
* csv file names ``train_ship_segmentations_v2.csv`` and ``train_ship_segmentations_v2_only_ship_images.csv``
* first contains all ship images including those without ships

#### YOLOv4 Tutorial
##### Youtube
* [YOLOv4 in the CLOUD: Install and Run Object Detector FREE GPU](https://www.youtube.com/watch?v=mKAEGSxwOAY)
* [YOLOv4 in the CLOUD: Build and Train Custom Object Detector FREE GPU](https://www.youtube.com/watch?v=mmj3nxGT2YQ)
* [How to Build a Custom YOLOv4 Object Detector using TensorFlow - License Plate Detector](https://www.youtube.com/watch?v=nOIVxi5yurE)
##### Github
* [The AI Guy](https://github.com/theAIGuysCode) This guy made some pretty nice tutorials for Yolo v3 and v4.

#### Useful Links
- [Airbus Ship Detection - Traditional v.s. Convolutional Neural Network Approach](http://cs229.stanford.edu/proj2018/report/58.pdf) by Ying Chen, Junwen Zheng, Zhengqing Zhou 
- [Lessons Learned from Kaggle’s Airbus Challenge](https://towardsdatascience.com/lessons-learned-from-kaggles-airbus-challenge-252e25c5efac)
- [Run Length Decoding](https://www.kaggle.com/chisanchensc/run-length-decoding-quick-start)


~codelover96
