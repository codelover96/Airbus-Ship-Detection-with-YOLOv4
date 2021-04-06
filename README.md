# Airbus-Ship-Detection-with-YOLOv4
Airbus Ship Detection Challenfe with YOLOv4 object detector
Back in 2019 Airbus published a challenge for ship detectio on Kaggle. Airbus provided a large dataset of satellite ship images from SPOT satellite.
There are many attempts on solving this challenge, published on Github. In this attempt I'm using YOLOv4 object detector. Other have used Mask R-CNN, Single Shot Detector etc.

#### Why YOLOv4
Altough YOLOv4 does not perform well when there are objects really close to each other which is the case for many images on this dataset, it is considered to be really fast. I chose to use yolo simply because of my familiarity with it in the past. In the future I plan on solving this problem with Mask R-CNN.

### More on the Dataset
[Airbus Ship Detection Challenge on Kaggle](https://www.kaggle.com/c/airbus-ship-detection)
