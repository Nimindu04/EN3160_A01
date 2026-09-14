# EN3160 Assignment 1 — Intensity Transformations and Neighborhood Filtering

This repository contains my solutions for **EN3160 Assignment 1** from the Department of Electronic and Telecommunication Engineering, University of Moratuwa.

The assignment focuses on fundamental **digital image processing techniques**, including intensity transformations, histogram processing, color-space manipulation, spatial filtering, image interpolation, image segmentation, and edge-preserving smoothing.

## 👨‍🎓 Student Information

* **Name:** Prishmika H.W.N
* **Index Number:** 230500N
* **Course:** EN3160
* **Assignment:** Assignment 1
* **Department:** Electronic and Telecommunication Engineering
* **University:** University of Moratuwa

## 📌 Topics Covered

The assignment includes the following image processing techniques:

1. **Piecewise Intensity Transformations**

   * Implementation of intensity transformation using lookup tables (LUTs)
   * Different transformation curves and their corresponding image outputs

2. **MRI Image Enhancement**

   * White matter accentuation
   * Gray matter accentuation
   * Histogram analysis of the transformed images

3. **Gamma Correction**

   * Conversion to LAB color space
   * Gamma correction of the L-channel
   * Comparison of original and corrected images
   * Histogram analysis

4. **Vibrance Enhancement**

   * HSV color-space processing
   * Saturation enhancement using a Gaussian-based transformation
   * Evaluation of different values of the parameter `a`

5. **Histogram Equalization**

   * Manual implementation of histogram equalization
   * Comparison of original and equalized images
   * Histogram analysis

6. **HSV-Based Image Segmentation**

   * Separation of foreground and background using the Saturation plane
   * Foreground extraction
   * Histogram equalization of the foreground

7. **Sobel Filtering**

   * OpenCV 2D filtering
   * Custom 2D convolution implementation
   * Separable 1D Sobel filtering
   * Numerical comparison between the filtering approaches

8. **Image Interpolation**

   * Nearest-neighbor interpolation
   * Bilinear interpolation
   * Normalized Sum of Squared Differences (SSD) comparison

9. **Image Segmentation and Background Enhancement**

   * GrabCut-based foreground segmentation
   * Foreground and background extraction
   * Gaussian blurring of the background

10. **Bilateral Filtering**

    * Gaussian filtering
    * OpenCV bilateral filtering
    * Custom bilateral filter implementation
    * MSE and PSNR-based quantitative comparison

## 🛠️ Technologies and Libraries

The implementation was developed using **Python** with the following libraries:

* Python
* NumPy
* OpenCV
* Matplotlib

## 📂 Repository Structure

```text
EN3160_A01/
│
├── images/
│   ├── q1.jpeg
│   ├── q2.jpeg
│   ├── q3.jpeg
│   ├── q4.jpeg
│   ├── q5.tif
│   ├── q6.jpeg
│   ├── q7.jpeg
│   ├── q9.jpeg
│   ├── q10.jpeg
│   ├── im01.png
│   ├── im01small.png
│   ├── im02.png
│   ├── im02small.png
│   ├── im03.png
│   ├── im03small.png
│   ├── im04.jpg
│   └── im04small.jpg
│
├── notebooks/
│   └── EN3160_A01.ipynb
│
├── README.md
└── ...
```

> The exact file structure may vary depending on the files included in the repository.

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Nimindu04/EN3160_A01.git
```

### 2. Navigate to the project directory

```bash
cd EN3160_A01
```

### 3. Install the required libraries

```bash
pip install numpy opencv-python matplotlib
```

### 4. Run the Jupyter Notebook

```bash
jupyter notebook
```

Open the assignment notebook and execute the cells sequentially.

## 📊 Key Results

Some important observations from the assignment include:

* Different piecewise intensity mappings can emphasize different intensity ranges.
* Gamma correction with **γ = 0.6** improves visibility in darker regions while maintaining the brighter regions.
* A vibrance parameter of **a = 0.6** produced the most visually pleasing result in the tested range.
* Histogram equalization improved overall image contrast and revealed additional image details.
* The Saturation plane was effective for separating the colorful foreground from the less colorful background.
* The custom separable Sobel implementation produced the same result as the OpenCV filtering approach, with a maximum absolute difference of `0`.
* Bilinear interpolation produced lower normalized SSD values than nearest-neighbor interpolation for all four tested image pairs.
* The custom bilateral filter achieved an **MSE of 29.0938** and **PSNR of 33.49 dB** compared with the OpenCV bilateral filter.

## 📈 Bilateral Filter Comparison

The final part compares Gaussian filtering with bilateral filtering and evaluates the custom bilateral filter against OpenCV's implementation.

| Metric | Custom vs OpenCV |
| ------ | ---------------: |
| MSE    |          29.0938 |
| PSNR   |         33.49 dB |

The results show that the bilateral filter provides better edge preservation than Gaussian filtering, while the custom implementation produces an output close to the OpenCV implementation.

## 🎯 Learning Outcomes

Through this assignment, I gained practical experience in:

* Implementing image intensity transformations
* Working with different color spaces such as LAB and HSV
* Performing histogram analysis and equalization
* Implementing convolution and spatial filters manually
* Understanding separable filters
* Comparing image interpolation methods quantitatively
* Performing foreground/background segmentation
* Implementing edge-preserving bilateral filtering
* Evaluating image-processing algorithms using numerical metrics

## 📚 Course

**EN3160 - Image Processing and Machine Vision **
Department of Electronic and Telecommunication Engineering
University of Moratuwa

## 🔗 Repository

GitHub: https://github.com/Nimindu04/EN3160_A01
