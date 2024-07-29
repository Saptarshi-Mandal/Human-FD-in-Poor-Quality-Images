# Impact of Image Preprocessing on Human Face Detection in Poor Quality Images

<p align="center">
  <img src="/Images/intro.png">
</p>
## Introduction

In the field of computer vision, accurate face detection is a critical challenge, particularly when dealing with low-quality images. This project investigates the impact of various pre-processing techniques, including image denoising, deblurring, and contrast enhancement, on the performance of face detection in poor-quality images.

## Features
- Implementation of various image pre-processing techniques
- Evaluation of face detection performance on low-quality images
- Comparative analysis of different pre-processing methods

## Pre-processing Techniques

1. ### Denoising Techniques
   i. **Wiener Filter**
   ii. **Principal Component Analysis (PCA)**
   iii. **Non-Local Means (NLM)**

2. ### Deblurring Techniques
   i. **Wiener Filter**

3. ### Contrast Enhancement Techniques
   i. **BBHE (Brightness Preserving Bi-Histogram Equalization)**
   ii. **RMSHE (Recursive Mean-Separate Histogram Equalization)**

## Classifier
- The **Haar Cascade Classifier** is used for face detection in this project.

## Dataset
The dataset used for this project is the [Face-Detection-Dataset](https://www.kaggle.com/datasets/fareselmenshawii/face-detection-dataset) available on Kaggle.


## Results and Analysis

### Performance Metrics
The performance of the face detection algorithm is evaluated using the following metrics:
- **Intersection over Union (IoU)**
- **Average Precision**
- **Average Recall**

The performance of the different pre-processing techniques on face detection are also compared using the above metrics.
We synthetically introduced white noise of variances ranging from 0.1 to 0.5 on the original clean images and then applied the different pre-processing techniques to analyse the performance on face detection.
<p align="center">
  <img src="/Results/result1.png" alt="Comparison of the different pre-processing techniques when white noise is applied on the images">
</p>
Similarly, instead of white noise, salt and pepper noise was introduced.
<p align="center">
  <img src="/Results/result2.png" alt="Comparison of the different pre-processing techniques when salt and pepper noise is applied on the images">
</p>
Lastly, we also tested the impact of image pre-processing by introducing gaussian blur along with white noise.
<p align="center">
  <img src="/Results/result3.png" alt="Comparison of the different pre-processing techniques when gaussian blur and white noise is applied on the images">
</p>

## Project Structure

```plaintext
├── Code
│   └── E9 241 Digital Image Processing Project 2023 (OH & SM).ipynb
├── Results
│   ├── Results.xlsx
│   ├── Results - Avg. IoU.png
│   └── Results - Avg. Recall.png
└── README.md
```
