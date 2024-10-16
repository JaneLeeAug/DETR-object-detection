# DETR-object-detection
## Overview
This project fine-tunes the DETR (DEtection TRansformers) model for object detection using custom data. The data is first converted into the COCO format, and a pre-trained model is used to speed up training.
## Image Inference with JSON Output Results

## Reproduce（Train）
#### Modify Parameters
1. Download pretrained model
* https://github.com/facebookresearch/detr?tab=readme-ov-file

Use change.py to change the num_class of the pretrained model.

2. In main.py, adjust the following parameters:
* output_dir: Directory for saving the trained model weights (.pth file).
* dataset_file: Path to the dataset.
* coco_path: Path to the COCO dataset.
* coco_panoptic_path: Path to the label files.
* resume: Path to the pre-trained weight file of step 1.

3. Start trainin
   ```bash
   python3 main.py
   ```
4. In your output_dir you can see the trained model
