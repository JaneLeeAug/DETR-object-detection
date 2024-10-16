# DETR-object-detection
## Overview
This project fine-tunes the DETR (DEtection TRansformers) model for object detection using custom data. The data is first converted into the COCO format, and a pre-trained model is used to speed up training.
## Image Inference with JSON Output Results

## Reproduce（Train）
#### Modify Parameters
In main.py, adjust the following parameters:

* --output_dir: Directory for saving the trained model weights (.pth file).
* --dataset_file: Path to the dataset.
* --coco_path: Path to the COCO dataset.
* --coco_panoptic_path: Path to the label files.
