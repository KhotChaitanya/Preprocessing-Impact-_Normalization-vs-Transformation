# Preprocessing Impact: Normalization vs Transformation

This project explores the effect of two preprocessing techniques — **Normalization** and **Power Transformation** — on the performance of **Logistic Regression** and **SVM** models. It uses **Principal Component Analysis (PCA)** to reduce features for visualization and model training.

---

## Objective

- Apply two preprocessing strategies: Normalization and Power Transformation
- Use PCA to reduce dimensionality from 4D to 2D for visualization
- Train and compare Logistic Regression and SVM on both preprocessed versions
- Visualize decision boundaries in PCA space
- Evaluate classification accuracy

---

## Dataset

- **Source:** `sklearn.datasets.load_iris()`
- **Total Samples:** 150
- **Features:** 4 numerical features (sepal length, sepal width, petal length, petal width)
- **Target Classes:** 3 (Setosa, Versicolor, Virginica)

---

## Preprocessing Techniques

| Step                 | Normalization             | Power Transformation       |
|----------------------|---------------------------|-----------------------------|
| Scaling              | MinMaxScaler (0–1)        | PowerTransformer (Yeo-Johnson) |
| Dimensionality       | PCA (n_components=2)      | PCA (n_components=2)        |

---

## Models Used

| Model                | Description                            |
|----------------------|----------------------------------------|
| Logistic Regression  | Linear classifier for multi-class      |
| Support Vector Machine (SVM) | Kernel-based classifier             |

---

## Results

| Preprocessing    | Model               | Accuracy |
|------------------|---------------------|----------|
| Normalization    | Logistic Regression | 96.67%   |
| Normalization    | SVM                 | 96.67%   |
| Transformation   | Logistic Regression | 93.33%   |
| Transformation   | SVM                 | 93.33%   |

---

## Visualizations

- **Distribution of Median House Value:**

![6_1](https://github.com/user-attachments/assets/35f5457d-8a67-4aff-bf1b-e24e19bf7d06)

- **Prediction vs Actual Transformed Model:**

![6_3](https://github.com/user-attachments/assets/449ba639-94fa-4219-b362-4068c2cd3d21)


- **Residual Plots: Linear Regression**

![6_2-1](https://github.com/user-attachments/assets/ca403038-4e10-433b-93ab-305e145a0219)


- **Residual Plots: Random Forest**

![6_2-2](https://github.com/user-attachments/assets/c50dcd0d-2d42-41d0-8e1c-131041a9f291)


- **Model Accuracy Comparison:**

![6_4](https://github.com/user-attachments/assets/b2d31321-806d-4f94-8ba9-700f9f0c55da)


- *No accuracy bar chart is included in this notebook*

---

## Conclusion

- **Normalization outperformed Power Transformation** slightly in this comparison.
- Both Logistic Regression and SVM performed well on the Iris dataset after PCA.
- PCA enabled 2D visualization of decision boundaries.
- Even with minimal preprocessing differences, classification performance varies.

---

## Skills Applied

- Data Preprocessing: Normalization, PowerTransformer
- Dimensionality Reduction: PCA
- Classification: Logistic Regression, Support Vector Machine
- Evaluation: Accuracy
- Visualization: Decision Boundary Plots

---

## How to Run

```bash
# Clone the repository
git clone https://github.com/yourusername/Preprocessing_Impact_Normalization_vs_Transformation

# Navigate to the project folder
cd Preprocessing_Impact_Normalization_vs_Transformation

# Launch the notebook
jupyter notebook Normalization_vs_Transformation.ipynb
