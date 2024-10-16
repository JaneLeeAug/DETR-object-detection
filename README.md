# DETR-object-detection
## Overview
This project fine-tunes the **DETR** (DEtection TRansformers) model for object detection using custom data. The data is first converted into the COCO format, and a pre-trained model is used to speed up training.
## Image Inference with JSON Output Results
#### 1. Download the trained model.
- [Download Trained Model](https://drive.google.com/file/d/1CYLJR5HcQF6qdpTDvlDPIRenx0mUg66G/view?usp=share_link)
#### 2. In infer.py, adjust the following parameters:
* model_path: Path to the trained model.
* data_dir: Directory for the images you wanna infere.
* output_file: Path for saving the result JSON file.
#### 3. Start inferencing
   ```bash
   python3 infer.py
   ```
#### 4. The result JSON file is saved in _output_file_.

## Reproduce
#### 1. Download a pretrained model
- [Download Pretrained Model](https://github.com/facebookresearch/detr?tab=readme-ov-file)

   And then use change.py to change the num_class of the pretrained model.

#### 2. In main.py, adjust the following parameters:
* output_dir: Directory for saving the trained model weights (.pth file).
* backbone: resnet101 or resnet50, depend on which of your pretrained model is.
* dataset_file: Path to the dataset.
* coco_path: Path to the COCO dataset.
* coco_panoptic_path: Path to the label files.
* resume: Path to the pre-trained weight file of step 1.

#### 3. Change the directory of the dataset to the format shown in below
   ```plaintext
   path/to/coco/
      train2017/       # train images
      val2017/         # val images
      annotations/
         instances_train2017.json
         instances_val2017.json
   ```
#### 3. Start trainin
   ```bash
   python3 main.py
   ```
#### 4. The trained model is saved in _output_dir_.
