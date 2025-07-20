# **Handwritten Digit Recognition for Postal Services**
---

## Overview

This project implements a multi-class classification system to recognize handwritten digits (0-9) from the MNIST dataset, simulating an automated sorting solution for postal services. The goal is to classify 28x28 pixel images of digits using a Random Forest Classifier with hyperparameter tuning via Grid Search and Random Search, and to visualize the accuracy results.

## Problem Statement

The handwritten digit recognition task aims to automate the sorting process for postal services by classifying scanned images of handwritten digits (0 through 9) on envelopes. This multi-class classification problem involves analyzing 28x28 pixel images from the MNIST dataset, which contains 70,000 samples, to accurately identify digits based on their pixel intensity values. The challenge lies in achieving high accuracy despite variations in handwriting styles, requiring effective model selection and hyperparameter tuning using techniques such as Grid Search and Random Search with a Random Forest Classifier. The goal is to develop a reliable system that minimizes manual sorting efforts, improves efficiency, and reduces errors in large-scale postal operations.

## Requirements

Python 3.x

**Required libraries:**

scikit-learn (for machine learning and dataset handling)
matplotlib (for visualization)


## Install dependencies using:
pip install scikit-learn matplotlib


## Usage

- Clone or download the repository.
- Navigate to the project directory.

**Run the script:**
python digit_recognition_tuning.py


**The script will:**

- Load and preprocess the MNIST dataset.
- Perform hyperparameter tuning with Grid Search and Random Search.
- Display accuracy scores and a bar chart comparing the results.


## Files

-digit_recognition_tuning.py: Main Python script containing the classification and visualization code.


## Results

- The output includes the best parameters and accuracy scores for both Grid Search and Random Search.
- A bar chart visualizes the accuracy comparison, with the y-axis ranging from 0 to 1.

## Notes

- The MNIST dataset is automatically fetched and contains 70,000 images (60,000 training, 10,000 testing).
- The code uses a subset of hyperparameters for efficiency; adjust param_grid or param_dist for more thorough tuning if needed.
- Expected accuracy ranges from 0.90 to 0.97 with the current setup.

## Future Improvements

- Experiment with deeper models like Convolutional Neural Networks (CNNs) for higher accuracy.
- Increase the range and number of hyperparameters for more robust tuning.
- Incorporate additional datasets or real-world postal images for enhanced generalization.

## Conclusion

The implementation of a Random Forest Classifier with hyperparameter tuning using Grid Search and Random Search on the MNIST dataset demonstrates a viable solution for handwritten digit recognition in postal services. The model achieved competitive accuracy, with Grid Search and Random Search yielding comparable results, typically around 0.90-0.97 depending on the parameter settings. The visualization of accuracy comparisons highlights the effectiveness of both tuning methods, providing insights for optimizing performance. This approach successfully addresses the real-life need for automation, offering a foundation for further improvements such as using deeper neural networks or larger datasets to enhance precision and scalability in postal sorting systems.
