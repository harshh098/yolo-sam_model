# yolo-sam_model
# Hybrid YOLO-SAM Model for Automated Plastic Bottle Detection in Aerial Imagery

## Overview

This project focuses on the automated detection of plastic bottles in aerial drone imagery using a hybrid deep learning approach. By combining the power of YOLOv8 for object detection with the Segment Anything Model (SAM) for precise segmentation, this model aims to enhance the accuracy and efficiency of plastic waste detection in oceanic and coastal regions.

## Objectives

- Train and evaluate a YOLOv8 model for single-class object detection (`plastic bottle`)
- Integrate the YOLOv8 detector with Meta AI's SAM for refined segmentation
- Perform inference on large-scale aerial imagery datasets
- Compare the performance of standalone YOLO and the hybrid YOLO-SAM model
- Apply active learning to iteratively improve the model’s performance

## Dataset

- **Primary Source**: UAV Plastic Detection Dataset
- **Format**: Images and CVAT-generated annotation CSV files
- **Annotations**: Only one class - `plastic bottle`
- **Frame Info**: 127 manually annotated frames extracted from 1700 frames across 32 drone videos

## Project Structure

project-root/ │ ├── data/ │ ├── images/ │ ├── annotations/ │ └── data.yaml │ ├── yolov8_training/ │ ├── train.py │ └── config.yaml │ ├── sam_integration/ │ ├── sam_utils.py │ ├── yolov8_sam_hybrid.py │ └── inference_pipeline.py │ ├── results/ │ ├── yolo_results/ │ └── hybrid_results/ │

