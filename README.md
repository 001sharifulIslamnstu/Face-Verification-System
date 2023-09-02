# Face Verification System

## Overview
The Face Verification System is a robust solution for detecting and recognizing faces in images and real-time webcam streams. This system leverages state-of-the-art deep learning models for face detection and recognition, making it suitable for various applications, including security, access control, and identity verification.

## Components

### Face Detection
- **Model Used:** Retinaface
- **Description:** Retinaface is a highly accurate and efficient face detection model that excels at detecting faces in images with varying scales, orientations, and occlusions.

### Object Detection
- **Model Used:** Yolov5
- **Description:** Yolov5 is employed for object detection, particularly for identifying objects or features alongside faces in input images.

### Face Recognition
- **Model Used:** Arcface (Resnet-50)
- **Description:** Arcface, based on the Resnet-50 architecture, is used for face recognition. It embeds detected faces into a high-dimensional feature space and performs recognition by comparing face embeddings.

## Configuration

- **Input Size:** 112x112 pixels
- **Distance Type:** Cosine distance (used for measuring similarity between face embeddings)

## Inference

### Inference on Test Image
To perform inference on a test image, use the following command:
```bash
python main.py --im --path=./test/8.jpg


