# Heartbeat Monitoring System

## Project Overview
This project analyzes heart rate data to detect abnormal heart conditions such as Bradycardia and Tachycardia.

The final goal of the project was to create additional datasets that help differentiate whether abnormal heartbeat patterns occur during:
- Rest condition
- Active/workout condition

The system classifies physiological state using only heart rate signal characteristics.

---

## Datasets Used
1. Normal Rest Dataset (~78 BPM)
2. Rest Bradycardia Dataset (~33 BPM)
3. Rest Tachycardia Dataset (~170 BPM)
4. Active Bradycardia Dataset (~50 BPM)
5. Active Tachycardia Dataset (~155 BPM)

---

## Features Added to Active Datasets
The active datasets were modified with realistic workout-related characteristics such as:
- Baseline wander from breathing movement
- Motion artefacts from body movement
- Increased signal noise
- Beat morphology changes during exercise

These features help the model distinguish active conditions from resting conditions.

---

## Machine Learning Classification
The project uses a Support Vector Machine (SVM) with RBF kernel to classify signals as:
- Rest condition
- Active/workout condition

### Features extracted:
- Mean BPM
- BPM variability
- Baseline wander power
- High-frequency noise power

---

## Results
The model successfully differentiated rest and active physiological states using signal characteristics and achieved approximately **80–100% classification accuracy** depending on signal overlap and added noise.

---

## Technologies Used
- MATLAB
- Signal Processing
- Machine Learning (SVM)
- JSON datasets
