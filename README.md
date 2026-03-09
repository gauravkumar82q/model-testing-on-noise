# Impact of Noise on Traditional Machine Learning Models

## 📌 Project Overview

This project demonstrates how **traditional machine learning models are sensitive to noise in data**.

We train a **Logistic Regression classifier** on a clean dataset and then evaluate its performance after adding **random noise** to the test data.

The goal is to show that **model accuracy decreases when noisy or corrupted inputs are introduced**, which highlights a limitation of traditional machine learning models.

---

## ⚙️ Technologies Used

* Python
* NumPy
* Matplotlib
* Scikit-learn

---

## 📊 Dataset

The dataset is generated using **Scikit-learn's `make_classification` function**.

Parameters used:

* `n_samples = 500`
* `n_features = 2`
* `n_informative = 2`
* `n_redundant = 0`
* `n_clusters_per_class = 1`

This creates a **synthetic binary classification dataset**.

---

## 🧠 Model Used

We use **Logistic Regression**, a traditional machine learning classification algorithm.

Key settings:

* `max_iter = 200`

The model is trained on **standardized data** using `StandardScaler`.

---

## 🔬 Experiment Steps

1. Generate a synthetic dataset.
2. Split the dataset into **training and testing sets**.
3. Normalize the features using **StandardScaler**.
4. Train a **Logistic Regression model** on clean training data.
5. Evaluate the model on **clean test data**.
6. Add **Gaussian noise** to the test dataset.
7. Evaluate the model again on the **noisy test data**.
8. Compare the accuracy of both scenarios using a **bar chart**.

---

## 📈 Results

The model typically shows:

| Dataset Type | Accuracy         |
| ------------ | ---------------- |
| Clean Data   | High accuracy    |
| Noisy Data   | Reduced accuracy |

This demonstrates that **traditional machine learning models can struggle when noise is introduced into input data**.

---

## 📊 Visualization

A bar chart is used to visualize the difference in accuracy between:

* Clean Data
* Noisy Data

This helps clearly show the **impact of noise on model performance**.

---

## ▶️ How to Run the Project

### 1️⃣ Install dependencies

```bash
pip install numpy matplotlib scikit-learn
```

### 2️⃣ Run the script

```bash
python main.py
```

The script will:

* Train the model
* Add noise to the dataset
* Display accuracy comparison
* Show a visualization graph

---

## 📚 Key Learning

This experiment highlights an important concept:

> Traditional machine learning models can perform well on clean data but may fail when inputs contain noise or adversarial perturbations.

This is one reason why **robust models and advanced techniques are required in real-world AI systems**.

---

## 🚀 Future Improvements

Possible improvements to this project:

* Test multiple models (SVM, Decision Trees, Random Forest)
* Experiment with different noise levels
* Visualize decision boundaries
* Implement adversarial attack simulations
* Compare with deep learning models

---

## 👨‍💻 Author

**Gaurav Kumar**
Backend Developer | AI & ML Enthusiast

GitHub: https://github.com/gauravkumar82q
