ECG Signal Compression using Walsh-Hadamard Transform (WHT)

This MATLAB project demonstrates how to compress and reconstruct an ECG (electrocardiogram) signal using the **Discrete Walsh-Hadamard Transform (WHT)** — a fast, non-sinusoidal, orthogonal transform commonly used in biomedical signal processing.

---

##  Project Overview

Efficient ECG signal storage and transmission is critical for medical devices and wearable health monitors. This project simulates an ECG signal, applies WHT to compress the data by keeping only the low-sequency coefficients, and reconstructs the signal using the inverse transform. The result is a denoised, compressed ECG waveform that preserves key features like R-peaks.

---

##  Results

### Original Noisy ECG and WHT Coefficients


- Most signal energy is concentrated in low-sequency components.
- This means the signal can be compressed while still retaining its shape and diagnostic features.

### Original vs Reconstructed ECG


- The red signal (reconstructed) closely follows the blue signal (original).
- Despite compression, key patterns like R-peaks are preserved.

---

##  Tools Used

- MATLAB
- Fast Walsh-Hadamard Transform (`fwht`)
- Signal visualization
- Root Mean Squared Error (RMSE) calculation

---

##  Files Included

| File Name                          | Description                                      |
|-----------------------------------|--------------------------------------------------|
| `ecg_compression.m`               | Main MATLAB script                               |
| `ecg_original_and_wht.png`        | Plot of ECG signal and WHT coefficients          |
| `ecg_original_vs_reconstructed.png`| Plot comparing original and reconstructed ECG   |
| `README.md`                       | Project description                              |

---

##  Key Concepts

- **WHT-based compression** reduces data size by keeping only significant coefficients.
- **Signal reconstruction** with inverse WHT shows minimal distortion.
- This method is suitable for **low-power medical devices** that need efficient data storage or transmission.

---

##  Future Enhancements

- Use real ECG data from PhysioNet or hospital datasets
- Implement R-peak detection and heart rate calculation
- Export compressed data for use in embedded systems

---

## About

This project was developed by Aakash Balamurugan as part of a biomedical signal processing exploration, showcasing how advanced transforms like WHT can be used in real-world health tech applications.
