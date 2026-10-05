# Aerial Target Classification Using Deep Learning

Deep learning project for classifying aerial targets into four categories using a custom CNN and transfer learning models. The project was developed and executed primarily in a Kaggle Notebook as part of an academic course assignment.

## Project Overview

This project was developed based on a provided academic problem statement. The objective was to build a base CNN and compare it with at least three transfer learning models for aerial target classification.

The original dataset is a YOLOv8-based object detection dataset. Since the assignment required an image classification task and classification metrics, the annotated bounding boxes were cropped from the source images and converted into individual 4-class classification samples.

## Dataset

The project uses the [Air Defense Object Detection Dataset (YOLOv8)](https://www.kaggle.com/datasets/caferfatihgltekin/air-defense-object-detection-dataset-yolov8) from Kaggle.

The original dataset contains four target classes:

- F16
- Helicopter
- Quadcopter
- Rocket

The dataset is originally formatted for object detection using YOLO annotations. Each labelled bounding box was extracted from its source image and converted into a single-label classification sample.

### Dataset Split

| Split | Source Images | Cropped Samples |
|---|---:|---:|
| Train | 6,318 | 7,453 |
| Validation | 1,354 | 1,603 |
| Test | 1,355 | 1,598 |

All cropped images were resized to **224 × 224 × 3** before model training and evaluation.

> **Note:** The dataset is not included in this repository. The notebook was developed and executed in the Kaggle environment using the dataset linked above.

## Models

The following models were trained and evaluated:

- Custom CNN
- VGG16
- ResNet50
- MobileNetV2

The transfer learning models use ImageNet-pretrained backbones with their classification heads trained for the four target classes.

## Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall / Sensitivity
- Specificity
- F1 Score
- ROC-AUC

All models were evaluated on the same held-out test set.

## Best Result

**ResNet50** achieved the best overall performance:

- **Accuracy:** 84.23%
- **ROC-AUC:** 0.9696

The overall performance ranking was:

**ResNet50 > VGG16 > MobileNetV2 > Custom CNN**

## Notebook

The complete implementation is provided in the Kaggle-based Jupyter Notebook:

`Aerial_Target_Classification.ipynb`

The notebook contains the dataset processing, bounding-box extraction, data augmentation, model training, hyperparameter tuning, evaluation, and generated results.

Because the notebook uses Kaggle-specific paths and the Kaggle environment, it is intended to be run on **Kaggle** with the required dataset rather than directly on a local machine.

## Project Report

The accompanying PDF report contains the complete methodology, model configurations, experiments, results, training curves, ROC curves, and discussion.

## Project Context

This repository contains the implementation and report for an academic course project. The work follows the requirements of the assigned problem statement while documenting the methodology and experimental results used to solve it.
