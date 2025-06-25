
# 🧠 `imp-RNN-working.py` – RNN for Impaired Motion Analysis

This script implements a Recurrent Neural Network (RNN) for analyzing **time-series data from impaired motor movements**. It is optimized for experiments involving motion tracking, rehabilitation assessment, or exergaming feedback.

---

## 🧾 Key Details

- **Script name:** `imp-RNN-working.py`
- **Functionality:** Train and evaluate a basic RNN/LSTM on sensor or movement data.
- **Use Case:** Impaired hand/limb motion prediction and rehabilitation analysis.

---

## 📦 Requirements

Install required packages:
```bash
pip install numpy pandas matplotlib torch scikit-learn
```

---

## 🚀 How to Run

```bash
python imp-RNN-working.py
```

---

## 📂 Expected Data Format

- `.csv` file with sequential input features (e.g. joint angles, accelerometer data)
- Time series should be properly ordered
- Labels or target values at the end of each sequence (if supervised)

---

## 🔍 Features

- Implements a basic RNN with optional LSTM cells
- Supports dynamic batch processing
- Includes visualization of training loss and model predictions

---

## 📈 Output

- **Training Loss Curve**
- **Actual vs Predicted Motion Trajectories**
- Optionally: save model checkpoints and metrics

---

## 🧪 Sample Use Case

```python
# Example: LSTM cell on stroke patient hand data
model = LSTM(input_size=6, hidden_size=64, num_layers=2)
```

Use this as a baseline for:

- Comparing healthy vs impaired limb data
- Visualizing recovery trends over time
- Plugging into an exergaming feedback loop

---

## 📌 Note

This is a **work-in-progress experiment** script—meant for rapid testing and adaptation. It is recommended to modularize into training and utility functions for production.
