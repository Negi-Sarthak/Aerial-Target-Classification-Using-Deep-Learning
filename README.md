# Aerial Target Classification Using Deep Learning

Deep learning project for classifying aerial targets into four categories using a custom CNN and transfer learning models.

## Project Overview

This project was developed as part of an academic course assignment based on a provided problem statement. The objective was to build a base CNN and compare it with at least three transfer learning models for aerial target classification.

The original dataset is a YOLOv8-based object detection dataset containing four target classes: **F16, Helicopter, Quadcopter, and Rocket**. Since the assignment required image classification metrics, the annotated bounding boxes were cropped from the original images and converted into a 4-class classification dataset.

## Models

- Custom CNN
- VGG16
- ResNet50
- MobileNetV2

The models were evaluated using accuracy, precision, recall, specificity, F1 score, and ROC-AUC.

## Best Result

**ResNet50** achieved the best overall performance with:

- **Accuracy:** 84.23%
- **ROC-AUC:** 0.9696

## Notebook

The project was developed and executed primarily as a **Kaggle Notebook**. The uploaded `.ipynb` contains the complete implementation, training process, evaluation, and generated results.

Because the notebook uses Kaggle-specific dataset paths and the Kaggle environment, it is intended to be run on **Kaggle** with the required dataset rather than directly on a local machine.

## Project Report

The accompanying PDF report provides the complete methodology, model configurations, experiments, results, and discussion.

## Project Context

This repository contains the implementation and report for an academic course project. The work follows the requirements of the assigned problem statement while documenting the methodology and experimental results used to solve it.
