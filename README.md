# PPG Signal Analysis and Anomaly Detection

This Jupyter Notebook (`main.ipynb`) performs analysis and anomaly detection on Photoplethysmogram (PPG) signals recorded during high resistance bike exercises. The notebook utilizes various data processing and machine learning techniques to filter, analyze, and detect anomalies in the PPG data.

## Table of Contents

- [Introduction](#introduction)
- [Data](#data)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Analysis](#analysis)
- [Results](#results)
- [Conclusion](#conclusion)

## Introduction

The purpose of this notebook is to process and analyze PPG signals to identify patterns and detect anomalies. PPG signals are used to measure heart rate and other cardiovascular metrics, making them valuable for health monitoring.

## Data

The data used in this analysis is sourced from the [Wrist PPG During Exercise](https://physionet.org/content/wrist/1.0.0/) dataset available on PhysioNet. The specific record analyzed is `wrist_ppg_during_exercise/s1_high_resistance_bike`.

## Dependencies

The following Python libraries are required to run the notebook:

- `pandas`
- `wfdb`
- `matplotlib`
- `numpy`
- `scipy`
- `tensorflow`
- `sklearn`

## Usage

To run the notebook, ensure you have all dependencies installed. You can install them using pip:

```bash
pip install pandas wfdb matplotlib numpy scipy tensorflow sklearn
```

Open the notebook in Jupyter and execute the cells sequentially to perform the analysis.

## Analysis

The notebook performs the following steps:

1. **Data Loading**: Loads the PPG signal data from the specified record.
2. **Signal Processing**: Applies a moving average filter and a Butterworth low-pass filter to the PPG signal.
3. **Anomaly Detection**: Uses an LSTM-based autoencoder to detect anomalies in the PPG signal.

## Results

- **Filtered Signals**: The notebook plots the original and filtered PPG signals.
- **Anomalies**: Anomalies in the PPG signal are detected and highlighted in the plots.
- **Reconstruction Error**: The reconstruction error is plotted to visualize the anomaly detection process.

## Conclusion

The analysis successfully filters the PPG signal and detects anomalies using an LSTM-based autoencoder. This approach can be used for real-time health monitoring and anomaly detection in PPG signals.