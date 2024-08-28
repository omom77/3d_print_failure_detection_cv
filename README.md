# YOLOV8 Model for 3D Print Failure Detection

## Table of Contents

- [Introduction](#introduction)
- [Sample Images from the Dataset](#sample-images-from-the-dataset)
- [Running the YOLOV8 Model](#running-the-yolov8-model)
  - [Setup Environment](#setup-environment)
  - [Run the `print_failure_detection.py`](#run-the-print_failure_detectionpy)
- [Dataset Creation](#dataset-creation)
  - [Dataset Preparation](#dataset-preparation)
  - [Data Preprocessing](#data-preprocessing)

## Introduction

This project features a Computer Vision model based on YOLOV8, designed to detect failed 3D prints. The model is trained on a custom dataset that includes both successful and faulty 3D prints, enhanced by integrating an additional dataset to ensure variety and robustness.

## Sample Images from the Dataset

<img src="https://github.com/omom77/3d_print_failure_detection_cv/blob/0c3c63bb79cfd435923b60855b161cbdefa3f076/training_results/sample_images_dataset/sample_image.png" width="25%" height="25%">

## Running the YOLOV8 Model

### Setup Environment

1. **Specify Python version and create a virtual environment:**

    ```bash
    python3.10 -m venv env
    ```

2. **Activate the virtual environment:**

    - On **Unix or MacOS:**

        ```bash
        source env/bin/activate
        ```

    - On **Windows:**

        ```bash
        .\env\Scripts\activate
        ```

### Run the `print_failure_detection.py`

Execute the following command to run the detection script:

```bash
python print_failure_detection.py
```

## Dataset Creation

### Dataset Preparation

- **Image Collection:**
  - Hand-collected images of both successful and faulty 3D prints, encompassing a wide range of scenarios.
  - Combined our own images with an additional dataset to enhance the variety and robustness of the training data.

- **Labeling:**
  - Each image was labeled to indicate whether it was an example of a successful or faulty 3D print.
  - This labeling enables the model to efficiently learn to distinguish between the two types of prints.

### Data Preprocessing
  - Applied contrast adjustments to improve image visibility.
  - Scaled all images to a standard size to ensure consistency and clarity.
  - Preprocessing steps are crucial for enhancing consistency and optimizing the training dataset.
---
