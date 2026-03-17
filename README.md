# anomaly-detection-system
# Real-Time Anomaly Detection System

## Overview

This project implements a real-time anomaly detection system using unsupervised machine learning techniques. It focuses on identifying unusual patterns in time-series data without relying on labeled training data.

The system simulates a streaming environment where data arrives sequentially, and anomalies are detected dynamically.

---

## Objectives

* Understand unsupervised learning for anomaly detection
* Apply feature engineering on time-series data
* Implement and compare multiple anomaly detection models
* Introduce adaptive thresholding for better detection
* Simulate real-time data processing

---

## Dataset

A synthetic time-series dataset is generated using a sinusoidal signal with added noise. Random anomalies are injected as spikes to simulate abnormal behavior.

---

## Methodology

### 1. Data Generation

* Created time-series data using sine wave + noise
* Injected anomalies at random points

### 2. Feature Engineering

* Rolling mean and rolling standard deviation
* Lag features to capture temporal dependencies

### 3. Models Used

* Isolation Forest
* One-Class SVM
* Local Outlier Factor

### 4. Anomaly Detection

* Models assign anomaly scores
* Predictions derived using model outputs

### 5. Adaptive Thresholding

* Normalized anomaly scores
* Applied percentile-based thresholding
* Controlled detection sensitivity

### 6. Real-Time Simulation

* Processed data sequentially
* Maintained rolling window buffer
* Generated predictions for incoming data points

### 7. Visualization

* Time-series plots with highlighted anomalies
* Model comparison charts

---

## Key Learnings

* Difference between supervised and unsupervised learning
* Importance of feature engineering in time-series problems
* Role of anomaly scores and threshold selection
* Trade-off between precision and recall in anomaly detection
* Basics of real-time data processing

---

## How to Run

1. Install dependencies:

```
pip install pandas numpy matplotlib scikit-learn
```

2. Run the notebook or script:

```
python run_pipeline.py
```

---

## Future Improvements

* Add real-time dashboard interface
* Implement alert notification system
* Extend to real-world datasets
* Experiment with deep learning-based anomaly detection

---

## Conclusion

This project demonstrates how anomaly detection systems can be built without labeled data and adapted for real-time scenarios. It serves as a foundation for understanding practical applications of unsupervised learning in monitoring systems.
