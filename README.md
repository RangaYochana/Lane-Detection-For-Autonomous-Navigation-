# Lane Detection System for Indian Roads

## Overview
This repository contains the implementation of a lane detection system designed specifically for Indian roads. The system has been optimized to handle common challenges such as broken lane markings and irregularities like expansion joints, often found on highways in India. The goal is to provide accurate and consistent lane detection by integrating Kalman and Exponential Moving Average (EMA) filters, along with Bayesian optimization to fine-tune parameters for the best results.

## Features
- **Lane Detection for Indian Roads:** Optimized for highways with broken lanes and expansion joints.
- **Hybrid Offset Calculation:** Combines Kalman and EMA filters for stable and accurate lane offset calculations.
- **Bayesian Optimization:** Uses Bayesian optimization to fine-tune the EMA's alpha parameter for optimal lane detection.
- **Real-time Performance:** Designed for real-time lane detection with an emphasis on maintaining high FPS (frames per second) while ensuring offset stability.

## Installation

### Prerequisites
Ensure you have the following installed on your machine:
- Python 
- OpenCV
- NumPy
- Matplotlib
  
## Optimization Approach

### Kalman Filter
The Kalman filter is used to predict the lane positions based on previous frame information, improving the accuracy and stability of lane offset calculations.

### Exponential Moving Average (EMA)
The EMA filter smooths the detected lane positions and adjusts them over time to avoid sharp jumps in lane detection.

### Bayesian Optimization
 Bayseain optimization was applied to determine the optimal alpha for EMA Filter, which was found to be 0.64.
## Results
 The hybrid approach outperforms Kalman and EMA individually, achieving a lane detection consistency of 99.88%. 


## Acknowledgements
- OpenCV for image processing and computer vision tools.
- NumPy for numerical operations.
- Matplotlib for visualizing results.

---

