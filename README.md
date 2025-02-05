---

# Brain Tumor Segmentation Using K-Means Clustering
---

This project involves segmenting brain tumors from MRI images using the K-Means clustering algorithm. The objective is to perform unsupervised image segmentation to isolate tumor regions from the MRI scans.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)

## Overview

Brain tumor segmentation is an important step in medical image analysis. This project applies K-Means clustering to grayscale MRI images to distinguish between healthy and tumor tissue. The algorithm is applied to MRI scans, dividing the image into clusters representing different regions in the brain.

## Dataset

The dataset consists of MRI images of the brain. An example image used for the project is named `Tr-gl_0126.jpg`. The images are read in grayscale for processing.

## Installation

### Prerequisites

Make sure you have the following installed:

- Python 3.6 or higher
- OpenCV
- NumPy
- Matplotlib

### Installation Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/Sankalpa0011/brain-tumor-segmentation-kmeans.git
   ```
2. Navigate to the project directory:
   ```bash
   cd brain-tumor-segmentation-kmeans
   ```

## Usage

To run the segmentation algorithm, follow these steps:

1. Place the MRI images you want to process in the `Datasets/test_images/` folder.
2. Open and run the Jupyter Notebook `Brain Tumor Segmentation K-Means Clusturing.ipynb`.
3. Example code for loading an image and applying K-Means clustering:

   ```python
   import cv2
   import matplotlib.pyplot as plt

   # Load a grayscale image
   img = cv2.imread("Datasets/test_images/Tr-gl_0126.jpg", 0)

   # Display the image
   plt.imshow(img, cmap="gray")
   plt.show()

   # Apply K-Means clustering here (further code provided in the notebook)
   ```

4. The segmented output will be displayed, highlighting the tumor regions in the MRI scan.

## Results

The project segments the tumor region from MRI images using unsupervised K-Means clustering. Below is an example of the output:

* (Include a sample image or result here.)

## Contributing

If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are welcome.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request
