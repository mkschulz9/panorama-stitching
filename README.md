# Panorama Stitching Project

Welcome to the Panorama Stitching Project repository! This repository contains a Jupyter Notebook (`.ipynb` file) that demonstrates how to stitch multiple images together to create a seamless panoramic image using computer vision techniques.

## Overview

This project explores creating a panoramic image by stitching overlapping photographs. The main steps involved are:

- **Feature Detection**: Utilizing the **Scale-Invariant Feature Transform (SIFT)** algorithm to detect keypoints and compute descriptors in each image.
- **Feature Matching**: Matching these keypoints between consecutive images using a brute-force k-nearest neighbors matcher and applying a ratio test to filter out unreliable matches.
- **Homography Estimation**: Computing homography matrices using the **RANSAC** algorithm to find the perspective transformations that align the images.
- **Image Warping and Blending**: Warping each image according to the computed homographies and blending them into a single panoramic image.

## Contents

- **`panorama_stitching.ipynb`**: The Jupyter Notebook containing the full code implementation, detailed explanations, and visualizations of each step in the panorama stitching process.
- **sample_imgs.zip**: A zip file containing the input images used in the notebook to demonstrate the stitching process.
