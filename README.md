# 🧠 MLP Depth Experiment – Wine Classification Tutorial

This repository contains the complete code and tutorial for analysing how **network depth affects the performance of a Multilayer Perceptron (MLP)**.  
The experiment uses the **Wine Classification Dataset** and compares four architectures with increasing hidden-layer depth.

---

## 📌 Project Goal

To investigate:

- How increasing neural network depth influences accuracy
- When depth improves learning, and when it causes degradation
- Why deeper models require caution on small datasets
- How to evaluate model performance using classification metrics

---

## Repository Structure

| File / Folder | Description |
|--------------|-------------|
| `MLP_Tutorial.ipynb` | Jupyter Notebook — full code for model training + plots |
| `Understanding_MLP_Depth_Using_Wine_Dataset.pdf` | Final written tutorial explaining the experiment |
| `README.md` | Documentation file (this file) |
| `LICENSE` | License file for usage rights |

> Ensure you upload the notebook + final tutorial document as required by assignment submission guidelines.

---

## Experiment Summary

MLP architectures tested:

| Model | Hidden Layers |
|-------|---------------|
| MLP-1 | (32) |
| MLP-2 | (64, 32) |
| MLP-3 | (128, 64, 32) |
| MLP-4 | (128, 64, 32, 16, 8) |

Metrics recorded:

- Train Accuracy
- Test Accuracy
- Number of iterations to converge
- Confusion Matrix + Classification Report

**Best performing architecture:**  
`128 → 64 → 32` (3 hidden layers)

---

## Key Findings

- Increasing depth **initially improves performance**
- The 3-layer MLP achieved the **best balance** of stability and generalisation
- The deepest 5-layer model **underperformed** due to overfitting + unstable gradients
- Depth helps **until it becomes too much** for small datasets

---

## How to Run

```bash
git clone https://github.com/Hemantpawar1996/MLP-Network-Depth-Tutorial.git
cd MLP-Network-Depth-Tutorial
jupyter notebook MLP_Tutorial.ipynb
```

## Make sure you have the following installed:
pip install numpy pandas scikit-learn matplotlib seaborn

## Visual Outputs Included
- Train vs Test Accuracy Bar Plot
- Confusion Matrix of Best Model
- Classification Report
- Summary Accuracy Table
All results demonstrate the depth-performance relationship in a clear, tutorial-style format.

License
This project is licensed under the MIT License.
You are free to use, modify and distribute — academic credit is appreciated.



