# Skin Detection Using Image Processing

This project implements a classical image processing approach for detecting human skin regions in images. Skin detection is a common preprocessing step in computer vision applications such as face detection, gesture recognition, and human tracking.

The system is based on YCbCr color space thresholding combined with morphological operations and connected component analysis to refine segmentation results. An alternative HSV-based approach was also explored and experimentally compared.

## Project Objectives
- Perform skin region segmentation using classical image processing techniques
- Analyze and compare YCbCr and HSV color spaces for skin detection
- Reduce noise and false positives using morphological filtering
- Evaluate segmentation performance using standard computer vision metrics

## Methodology
- Convert input images to the YCbCr color space
- Apply empirically selected Cb and Cr threshold ranges for skin detection
- Refine binary masks using morphological opening, closing, and smoothing
- Retain the largest connected component to minimize background noise
- Process images in batch mode with automated output generation

## Evaluation
The algorithm was evaluated on 1,118 images with corresponding ground-truth masks using the following metrics:
- Accuracy
- Precision
- Recall
- F1 Score
- Intersection over Union (IoU)

### Average Results
- Accuracy: 91.49%
- IoU: 75.35%

The method performs well on well-lit images, with reduced accuracy in cases of low lighting or skin-colored backgrounds.

## Tools and Technologies
- Python
- OpenCV
- NumPy
- Pandas
- Matplotlib

## Notes
This project focuses on classical image processing techniques and does not use machine learning or deep learning models. It is intended for academic and educational purposes.
