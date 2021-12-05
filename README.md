# Kangaroo-detector

![alt text](https://github.com/mziad97/Kangaroo-detector/blob/main/gif_frame_006.jpg)

## The Detection model
 it's "SSD ResNet50 V1 FPN 640x640 (RetinaNet50)". The checkpoints (weights) can be found at [object detection zoo](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md).

I've fine-tuned the box and class heads, and kept weights of the feature extractor layers.

## used utilities from [object detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2.md)
1. config_util: to import the model configuration from pipeline_file
2. visualization_utils: to draw the bounding boxes, classes, and scores on the image2
3. colab_utils: to annotate the objects in the image
4. model_builder: build the model from the its configuration

## Dataset: 
Used a subset (6 images) for training, and 17 images for testing from this dataset: [kangaroo dataset](https://www.kaggle.com/hugozanini1/kangaroodataset)
