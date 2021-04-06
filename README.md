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
* Those subsets contain images with and without ships
* Includes 2 csv files one containing the image name and the encoded pixels in Run Length Encoding
* csv file names ``train_ship_segmentations_v2.csv`` and ``train_ship_segmentations_v2_only_ship_images.csv``
* first contains all ship images including those without ships

#### My process
* Copied only ship images from train subset with ``ship_images_copying.py``
* Converted Run Length Encoding for every ship in train subset, to bounding boxes and finally to YOLO format. ``rle-to-boxes.py``
* used this tool [Convert-YOLO-to-PascalVOC](https://github.com/carolinepacheco/convert-yolo-to-pascalvoc)
* *to be continued..*

#### Results
![Sample ship image](https://github.com/codelover96/Airbus-Ship-Detection-with-YOLOv4/blob/main/0a89c4e4b_558x558.jpg)
![Sample of Yolo v4 Results](https://github.com/codelover96/Airbus-Ship-Detection-with-YOLOv4/blob/main/0a89c4e4b_results.png)
#### Mean Average Precision

```calculation mAP (mean average precision)
 Detection layer: 139 - type = 28 
 Detection layer: 150 - type = 28 
 Detection layer: 161 - type = 28 
10640
 detections_count = 57677, unique_truth_count = 18295  
class_id = 0, name = ship, ap = 79.47%   	 (TP = 14342, FP = 4340) 

 for conf_thresh = 0.25, precision = 0.77, recall = 0.78, F1-score = 0.78 
 for conf_thresh = 0.25, TP = 14342, FP = 4340, FN = 3953, average IoU = 61.49 % 

 IoU threshold = 50 %, used Area-Under-Curve for each unique Recall 
 mean average precision (mAP@0.50) = 0.794678, or 79.47 % 
Total Detection Time: 225 Seconds
```

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

#### Notice
This repo is not complete. There are many additinos to be made. Like adding source files and displaying final results.

~codelover96
