# 📊 MNIST Digit Classification: CNN Model Comparison using TensorFlow & Keras

This project demonstrates how to build, train, and compare two convolutional neural network (CNN) models on the MNIST handwritten digits dataset using TensorFlow and Keras.

---

## 🚀 Project Goals

- Build two different CNN architectures  
- Train both models on the MNIST dataset  
- Compare their performance (accuracy & validation)  
- Visualize and interpret results  

---

## 📁 Dataset: MNIST

- **Type**: Handwritten digits (grayscale images)  
- **Shape**: 28x28 pixels  
- **Classes**: 10 (digits 0–9)  
- **Size**: 60,000 training images, 10,000 test images  

---

## 🧠 Model Architectures

### 🔸 Model A: Simple CNN
- Conv2D (32 filters, 3x3, ReLU)  
- MaxPooling2D (2x2)  
- Flatten  
- Dense (64 units, ReLU)  
- Dense (10 units, Softmax)  

### 🔸 Model B: Deeper CNN with Dropout
- Conv2D (64 filters, 3x3, ReLU)  
- Conv2D (64 filters, 3x3, ReLU)  
- MaxPooling2D (2x2)  
- Dropout (0.25)  
- Flatten  
- Dense (128 units, ReLU)  
- Dropout (0.5)  
- Dense (10 units, Softmax)  

---

## ⚙️ Training Configuration

| Parameter           | Value                          |
|---------------------|--------------------------------|
| Epochs              | 5                              |
| Validation Split    | 20%                            |
| Optimizer           | Adam                           |
| Loss Function       | Sparse Categorical Crossentropy |
| Evaluation Metric   | Accuracy                       |

---

## 📈 Evaluation Results

| Model   | Test Accuracy (%) |
|---------|-------------------|
| Model A | 98.30%            |
| Model B | 99.04%            |

---

## 📊 Validation Accuracy Visualization

Model B, being deeper and including dropout layers, achieved higher validation accuracy and generalization compared to Model A.

<img width="585" height="455" alt="image" src="https://github.com/user-attachments/assets/4e5154f4-1adc-4fa6-9af4-2d09269d2b04" />



---

## 📌 Conclusion

- **Model A**: Lightweight, fast to train, good for basic applications  
- **Model B**: Better performance due to depth and regularization (Dropout)  

### 🔧 Future Improvements

- Add Batch Normalization  
- Implement Data Augmentation  
- Perform Hyperparameter Tuning  

---

## 🧪 Requirements

```
pip install tensorflow scikit-learn matplotlib numpy
```

## Folder Structure
```
dna_project/
├── main.py             # Main training script
└──README.md                    # This file
```

