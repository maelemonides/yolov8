# YOLOv8 Training and Detection

This repository contains code for training and running object detection using YOLOv8, implemented using the Ultralytics library. It provides scripts for training the model on custom datasets and performing inference on images. Additionally, there is a Streamlit web application hosted on Google Colab for interactive inference.

## Requirements

- Python 3.x
- PyTorch
- Ultralytics library
- COCO dataset (for training)

Install the required dependencies using pip:

```
pip install ultralytics
```

## Usage

### Training

To train the YOLOv8 model, use the following command:

```
python train.py --data coco128.yaml --epochs 5 --imgsz 640
```

- `--data`: Path to the dataset configuration file (e.g., `coco128.yaml`).
- `--epochs`: Number of training epochs.
- `--imgsz`: Input image size.

### Inference

To perform object detection on images, run:

```
python detect.py --source /path/to/images --weights yolov8n.pt
```

- `--source`: Path to the directory containing images.
- `--weights`: Path to the trained model weights file.

### Streamlit Web Application

An interactive Streamlit web application is available for performing inference on images. The application is hosted on Google Colab. To use it, follow these steps:

1. Open the [YOLOv8 Streamlit App]
2. Follow the instructions provided in the notebook to upload images and perform inference using the trained YOLOv8 model.

## Dataset Preparation

Make sure to organize your dataset in the COCO format and create a YAML configuration file specifying the dataset details such as paths to images and labels.

## Results

After training, the model weights and training logs will be saved in the `runs` directory. You can visualize the training progress and evaluate the model's performance using TensorBoard.


![wamp1](https://github.com/maelemonides/yolov8/assets/101704314/3d48a270-262e-4ced-a90d-768d20e0c3bc)




![wamp2](https://github.com/maelemonides/yolov8/assets/101704314/b23840af-5359-4730-ac28-db8f847e6e61)

![wamp 3](https://github.com/maelemonides/yolov8/assets/101704314/1a5a8afd-3d13-4bbe-9e8a-06457e4d3d46)
![wamp 4](https://github.com/maelemonides/yolov8/assets/101704314/2de6f77d-2b65-4ad0-9e80-bed967184a60)

https://wandb.ai/mael-emonides/ultralytics?nw=nwusermaelemonides
