
# Brain Tumor Segmentation using YOLO v8

## Overview

This repository contains the implementation of a YOLO v8 model for brain tumor segmentation, achieving **99.4% mAP**.

## Dataset

- **Source:** [Roboflow Brain Tumor Dataset](https://app.roboflow.com/data-science-tnitc/brain-tumor-40crk-zgelw-baoel/visualize/1)
- **Classes:** Tumor, Non-Tumor

## Model Performance

- **mAP:** 99.4%

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/brain_Tumor_Segmentation.git
   cd brain_Tumor_Segmentation
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset from [Roboflow](https://app.roboflow.com/data-science-tnitc/brain-tumor-40crk-zgelw-baoel/visualize/1) and place it in the `data/` directory.

## Usage

- Train the model:
  ```bash
  python train.py --data data/brain_tumor.yaml --epochs 100 --img-size 640
  ```

- Evaluate the model:
  ```bash
  python val.py --data data/brain_tumor.yaml --weights path/to/weights.pt
  ```

- Run inference:
  ```bash
  python detect.py --source path/to/image_or_folder --weights path/to/weights.pt --img-size 640
  ```

## License

This project is licensed under the MIT License.

---
