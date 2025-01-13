
**__NOTE: Transformer architecture will work much better in this case, I suggest you train or finetune a pretrained transformer from hugging face.__**

# Vibrational Analysis of a DC Motor for Fault Detection

Detecting faults in rotating machinery is critical for minimizing maintenance costs and avoiding production downtimes. This project uses **vibration data** and **machine learning algorithms** to identify unbalanced states in the shaft of a DC motor with high accuracy.

---

## ⚙️ Project Overview

- **Objective**: Early detection of unbalances in rotating shafts to prevent damage and extend machinery lifespan.
- **Experimental Setup**:
  - **Hardware**: LabVolt Universal DC Motor (8254-00), MPU6050 accelerometer, and Arduino Uno.
  - **Dataset**: Over **100 million vibrational data points** generated using VBA code.
- **Machine Learning Approaches**:
  - **Convolutional Neural Networks (CNN)**: Achieved **97.2% accuracy**.
  - **Fast Fourier Transform (FFT)**: Reached **84% accuracy**.

---

## 📊 Key Features

### Dataset
- Captured vibration data along three axes (**x, y, z**) using the MPU6050 accelerometer.
- Covers:
  - Five different unbalance strengths.
  - Various rotational speeds (RPM).
- **CSV Format**:
  - Columns: `Input Voltage (V)`, `Vibration_x`, `Vibration_y`, `Vibration_z`.
  - Sampling Rate: **4096 values/sec** for CNN, **2048 values/sec** for FFT.

### Algorithms
1. **Convolutional Neural Networks (CNN)**:
   - Recognizes patterns in vibration data for classification tasks.
   - Delivers high accuracy and effective fault detection.
2. **Fast Fourier Transform (FFT)**:
   - Converts time-series data into the frequency domain.
   - Performance varies with smaller datasets and transformations.

---

## 🛠️ Results and Insights

- **CNN** demonstrated superior performance with **97.2% accuracy**.
- **FFT** achieved acceptable results but struggled with smaller datasets.
- Highlighted the importance of:
  - **Data augmentation**: Expanding the dataset from 20,000 to 100 million values.
  - **Robust feature extraction**: Ensuring meaningful and generalized insights.

---

## 🚀 Applications

- **Predictive Maintenance**: Identifying faults in industrial machinery before failures occur.
- **Real-Time Monitoring**: Detecting anomalies during operation to avoid downtime.
- **Mechanical Reliability**: Enhancing the longevity and safety of production systems.

---

## 📈 Future Work
- Will train or finetune a transformer this time.
- Combining CNN and FFT models for improved speed-dependent fault detection.
- Exploring **explainable AI (XAI)** techniques for better interpretability.
- Applying ensemble learning techniques for enhanced prediction accuracy.

---

## 📜 Citation
If you use this project or dataset in your research, please cite the following:
> **[Anser Zuha Ali]**. "Vibrational Analysis of a DC Motor for Fault Detection." *Technical Report*, NUST, 2025.

---

Feel free to suggest edits or improvements for better insights!
