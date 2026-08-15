````markdown
# 🍎 Apple Leaf Disease Classification Using CNN

A Convolutional Neural Network (CNN) project for classifying apple leaf images into four categories using the PlantVillage dataset.

## Classes

- Apple Scab
- Black Rot
- Cedar Apple Rust
- Healthy

## Dataset

PlantVillage Dataset:  
https://github.com/spMohanty/PlantVillage-Dataset

## Model

- Framework: TensorFlow / Keras
- Input Size: 256 × 256 RGB
- Optimizer: Adam
- Loss: Sparse Categorical Crossentropy
- Epochs: 20
- Output Classes: 4

## CNN Structure

```text
Input: 256 × 256 × 3
        ↓
Conv2D (16 filters, 3×3, ReLU)
        ↓
MaxPooling2D
        ↓
Conv2D (32 filters, 3×3, ReLU)
        ↓
MaxPooling2D
        ↓
Conv2D (16 filters, 3×3, ReLU)
        ↓
MaxPooling2D
        ↓
Flatten
        ↓
Dense (256 neurons, ReLU)
        ↓
Dense (4 neurons, Softmax)
        ↓
Output: 4 Classes
````

## Results

| Metric     | Accuracy |
| ---------- | -------: |
| Training   |   99.46% |
| Validation |   95.16% |
| Test       |   93.13% |

## Project Structure

```text
├── models/
│   └── imageclassifier.keras
├── notebooks/
│   └── CNN.ipynb
├── Results/
│   ├── accuracy.png
│   └── loss.png
├── README.md
└── .gitignore
```

## Author

**Manas Kedia**

```
```
