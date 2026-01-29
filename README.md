# LAB 3: Effect of L1, L2, and Elastic Net Regularization on Model Training

## 📌 Aim
To study and compare the effect of L1, L2, and Elastic Net regularization techniques on a deep learning model, and to analyze how regularization helps in reducing overfitting and improving performance on unseen data.

---

## 📖 Introduction
Deep learning models with high capacity often suffer from overfitting, where the model performs very well on training data but poorly on unseen data. Regularization techniques are used to control model complexity by adding penalty terms to the loss function.  
This lab demonstrates the effect of **L1**, **L2**, and **Elastic Net** regularization on model training, validation, and generalization.

---

## 📂 Dataset Used
**Breast Cancer Wisconsin Dataset**
- Source: `sklearn.datasets`
- Number of features: 30
- Type: Binary classification (Benign / Malignant)

This dataset is suitable for studying overfitting and regularization due to its moderate size and numerical features.

---

## 🛠️ Technologies Used
- Python  
- PyTorch  
- Scikit-learn  
- Matplotlib  

---

## 🧠 Model Architecture
A deep neural network with multiple hidden layers was intentionally used to create overfitting.  
The model includes:
- Fully connected layers
- ReLU activation
- Sigmoid activation for binary classification

---

## 🔬 Experiments Performed

### 1️⃣ Model Without Regularization
- Achieved very high training accuracy
- Showed higher validation loss
- Clear evidence of overfitting

### 2️⃣ L2 Regularization (Weight Decay)
- Applied using `weight_decay` in the optimizer
- Reduced weight magnitude
- Improved validation performance
- Reduced overfitting

### 3️⃣ L1 Regularization
- Added manually to the loss function
- Encouraged sparsity by driving some weights to zero
- Reduced model complexity

### 4️⃣ Elastic Net Regularization
- Combination of L1 and L2 regularization
- Balanced sparsity and stability
- Achieved best generalization performance

---

## 📊 Results and Analysis
- The unregularized model overfitted the training data
- L2 regularization improved stability and generalization
- L1 regularization reduced unnecessary features
- Elastic Net provided the best trade-off between bias and variance

Training and validation accuracy/loss curves were plotted to visualize overfitting and the impact of regularization.

---

## ✅ Conclusion
This lab demonstrates that regularization is an essential technique in deep learning to prevent overfitting. Among the techniques studied, Elastic Net provided the most balanced performance by combining the advantages of both L1 and L2 regularization.

---

## 📁 How to Run
1. Clone the repository
2. Install required libraries
3. Run the Python script or Jupyter notebook
4. Observe training, validation metrics, and plots

---

## 👨‍🎓 Author
**Abhishek Kumar**  
BCA/ MSc – Artificial Intelligence & Machine Learning  

---

## 📌 Note
This project is developed purely for academic and learning purposes.
