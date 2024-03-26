# Automated Food Segmentation System

This repository contains Python code implementing a multi-step image segmentation for food-related images. The system aims to efficiently and accurately segment food items from images, facilitating automated food analysis, dietary assessment, and nutritional analysis.

## Objective

The primary objective of this research is to implement an efficient and accurate approach to food recognition, crucial for automated food analysis systems. The system employs computer vision techniques and algorithms to segment food items from images and evaluate segmentation quality using the mean Intersection over Union (mIoU) metric.

## Methodology

The system's workflow consists of the following steps:

1. **Preprocessing**: Gamma correction and normalization to enhance image quality.
2. **GrabCut Algorithm**: Iteratively refines a segmented mask to isolate food items.
3. **Mean Shift Algorithm**: Further segments regions obtained from GrabCut, improving segmentation results.
4. **Post-processing**: Morphological operations refine segmentation.
5. **Evaluation**: Calculates mIoU metric comparing processed segmentation with ground truth images.

## Libraries/Functions

The code utilizes the following libraries and functions:

- **cv2 (OpenCV)**: For image manipulation, segmentation algorithms (GrabCut, Mean Shift), morphology operations, and reading/writing images.
- **numpy**: For numerical computing and array manipulation.
- **matplotlib.pyplot**: For generating visualizations such as displaying images and creating subplots.
- **cv2.grabCut()**: Performs GrabCut algorithm for image segmentation.
- **cv2.pyrMeanShiftFiltering()**: Applies Mean Shift filter for image segmentation.
- **cv2.cvtColor()**: Converts color image to grayscale.
- **cv2.morphologyEx()**: Applies morphological operations to refine segmentation.

## Implementation

The Python code in this repository provides a systematic pipeline for food segmentation and evaluation in images. It iterates over specific images, performs segmentation, calculates mIoU scores, and displays segmented output alongside ground truth for visual comparison.

## Results

The algorithm underwent extensive testing on a dataset comprising 2135 food images, showcasing its performance in segmenting various food items. An average Intersection over Union (IoU) score of 0.57 was achieved, indicating a moderate level of accuracy in delineating food items from the background. 

## Potential Applications

This implementation serves as a comprehensive framework for image segmentation evaluation in food-related domains. It is essential for research in automated food recognition, analysis, and dietary assessment.

