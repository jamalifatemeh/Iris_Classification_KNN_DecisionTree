
# Iris Dataset Classification using KNN & Decision Tree

This project uses the **Iris dataset** to compare the performance of **K-Nearest Neighbors (KNN)** and **Decision Tree** classifiers. The goal is to classify iris species based on their flower measurements and determine which model performs best.

---

## 📊 Dataset Overview

The Iris dataset consists of 150 samples across three species:

- **Setosa**
- **Versicolor**
- **Virginica**

Each sample has 4 features:

- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

---

## ⚙️ Implementation Steps

### 1. Data Preparation
- Loaded Iris dataset using `sklearn.datasets`.
- Created a `DataFrame` and mapped numeric labels to species names.

### 2. Visualization
- Visualized sepal and petal relationships using scatter plots.
- Compared mean feature values for each species.

### 3. KNN Model
- Trained **KNN classifier** with `k=5`.
- Used **train/test split** with 30% for testing.
- Evaluated accuracy and generated a classification report.
- Ran KNN for `k=1` to `k=30` to find the optimal value based on test accuracy.
- Found **best k = 5**, achieving **accuracy = 0.97**

### 4. Decision Tree Model
- Trained a **Decision Tree classifier** on the same data split.
- Achieved **accuracy = 0.97**
- Visualized the decision tree using `plot_tree`.

---

## 🧪 Results

| Model          | Best Parameters | Test Accuracy |
|----------------|-----------------|----------------|
| KNN            | k = 5           | 0.97           |
| Decision Tree  | default         | 0.97           |

Both models performed equally well. KNN is simpler and non-parametric, while Decision Trees offer better interpretability.

---

## 📦 Dependencies

Make sure the following packages are installed:

```bash
pip install numpy pandas scikit-learn matplotlib
```

---

## 🚀 How to Run

1. Clone the repo:

```bash
git clone https://github.com/your-username/iris-knn-decisiontree.git
cd iris-knn-decisiontree
```

2. Run the script:

```bash
python iris_classification.py
```

---

## 📂 File Structure

```
iris-knn-decisiontree/
├── iris_classification.py
├── README.md
└── assets/
    └── [optional charts or figures]
```

---

## 📌 Conclusion

This project demonstrates a hands-on comparison of two classic classification models — KNN and Decision Tree — on a well-known dataset. It highlights:

- How to tune hyperparameters (K in KNN)
- How to visualize performance trends
- The simplicity and effectiveness of tree-based models

---

## 📄 License

MIT License.

---

🌸 Pattern recognition in petals and pixels 🌸
