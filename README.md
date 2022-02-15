# Global-Wheat-Detection
Use of deep learning to detect wheat heads from crops.

The project is based on this Kaggle Competition: https://www.kaggle.com/c/global-wheat-detection.

## DATA
**Data Format:** The data is images of wheat fields, with bounding boxes for each identified wheat head. Not all images include wheat heads / bounding boxes. The images were recorded in many locations around the world.

The CSV data is simple - the image ID matches up with the filename of a given image, and the width and height of the image are included, along with a bounding box. There is a row in train.csv for each bounding box. Not all images have bounding boxes.

**Goal:** The goal is to predict bounding boxes around each wheat head in images that have them. If there are no wheat heads, you must predict no bounding boxes.

**FILE STRUCTURE:**

1. train.csv - the training data
2. sample_submission.csv - a sample submission file in the correct format
3. train.zip - training images
4. test.zip - test images

**Fields in csv:**

1. image_id - the unique image ID
2. width, height - the width and height of the images
3. bbox - a bounding box, formatted as a Python-style list of [xmin, ymin, width, height].

## TRAINING
We have trained yolov5 model on this dataset. Training is perfomed on google colab.

**YOLOv5 Model:** https://github.com/ultralytics/yolov5

## INPUT : 
![53f253011](https://user-images.githubusercontent.com/71933031/153757117-372266ab-06eb-47f7-ae7f-ecdb7551cbaf.jpg)

## OUTPUT :
![download](https://user-images.githubusercontent.com/71933031/153757124-c88d0465-3387-4798-98d8-5a39dad766c0.jpg)

## Demonstration
https://user-images.githubusercontent.com/71033672/154047139-abc01392-6abe-4513-a6bd-bb81bf98b302.mp4
