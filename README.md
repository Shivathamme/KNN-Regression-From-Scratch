# KNN Regression from Scratch

This project presents an end-to-end implementation of the **K-Nearest Neighbors (KNN) regression algorithm from scratch** using Python and NumPy.  
The objective is to predict diamond prices based on their features and to compare the scratch implementation with Scikit-learn’s optimized KNN regressor.

---

## 📊 Dataset
- **Dataset:** Diamonds Dataset
- **Target Variable:** `price`
- **Categorical Features:** `cut`, `color`, `clarity`
- **Numerical Features:** `carat`, `depth`, `table`, `x`, `y`, `z`

---

## 🛠️ Tools & Technologies
- Python
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook

---

## 🔄 Project Workflow

1. **Data Loading**
   - Loaded the dataset using Pandas.

2. **Train–Test Split**
   - Split the data into training and testing sets using a 75:25 ratio.

3. **Data Preprocessing**
   - One-Hot Encoding for categorical variables.
   - Feature scaling for numerical variables using StandardScaler.

4. **KNN Regression from Scratch**
   - Implemented Euclidean distance manually.
   - Computed distances between test points and all training samples.
   - Selected the k-nearest neighbors.
   - Predicted prices using the average of neighbor values.

5. **Model Evaluation**
   - Evaluated the model using:
     - Mean Absolute Error (MAE)
     - Root Mean Squared Error (RMSE)

6. **Model Comparison**
   - Trained and evaluated `KNeighborsRegressor` from Scikit-learn.
   - Compared results with the scratch implementation.

---

## ⚡ Performance Note
The scratch KNN implementation was evaluated on the **entire test dataset**.  
While computationally expensive, this approach ensures a complete and fair evaluation of the algorithm’s performance.

---

## 📈 Results
- Scratch KNN and Scikit-learn KNN produced comparable error metrics.
- Scikit-learn KNN executed significantly faster due to internal optimizations.
- The scratch implementation demonstrates a strong understanding of KNN fundamentals.

---

## 🧠 Key Learnings
- Working principles of distance-based learning algorithms.
- Importance of feature scaling in KNN.
- Performance trade-offs between scratch implementations and optimized libraries.
- Handling categorical and numerical features effectively.

---

## 🚀 Future Improvements
- Optimize scratch KNN using vectorization.
- Experiment with different values of k.
- Implement weighted KNN.
- Add cross-validation.
