# TAWQ — Smart Swimmer Detection System

## Overview
TAWQ is an AI-powered computer vision project designed to support maritime search and rescue by detecting and locating swimmers in aerial drone images.

## The Problem
Detecting swimmers in large ocean areas is challenging because people appear very small in drone images and can be difficult to distinguish from waves and water reflections.

## Our Solution
We developed a swimmer detection system using YOLO object detection models. The system identifies swimmers, draws bounding boxes around them, and counts detected individuals to assist rescue teams.

We compared **YOLO11s and YOLO26s**, performed hyperparameter tuning, and selected **YOLO26s** based on its better evaluation results.

## Dataset
We used the [SeaDronesSee Object Detection Dataset](https://seadronessee.cs.uni-tuebingen.de/), adapted to focus on the **swimmer** class.

## Live Demo

**[Try TAWQ](https://tawq-demo.onrender.com/)**

## Presentation

**[View Presentation](./tawq-presentation.html)**


| Split | Images |
|---|---:|
| Training | 5,000 |
| Validation | 1,000 |
| Testing | 1,000 |
| **Total** | **7,000** |

## Project Files

| File | Description |
|---|---|
| `preprocessing_TOWQ (1).ipynb` | Dataset preparation and preprocessing |
| `Yolo11TrainingNotebook.ipynb` | YOLO11 training and tuning |
| `Yolo11_modelsVal.ipynb` | YOLO11 validation and model comparison |
| `Baseline(Yolo26).ipynb` | YOLO26 baseline training |
| `Tuned(Yolo26) (1).ipynb` | YOLO26 hyperparameter tuning |
| `Final_Model_Evaluation.ipynb` | Final model evaluation and comparison |
| `tawq-presentation.html` | Project presentation |



## Technologies
Python · Ultralytics YOLO · PyTorch · Google Colab · OpenCV
