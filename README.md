# NLU_sem2
# Sports vs. Politics Text Classifier

# 📌 Project Overview
This project implements a machine learning system to classify text documents into two categories: **Sports** and **Politics**. It utilizes the `20newsgroups` dataset and compares the performance of five different algorithms using a **Bag of Words** feature representation.

# 📂 Dataset
 **Source:** [20 Newsgroups Dataset](http://qwone.com/~jason/20Newsgroups/) (via Scikit-learn)
 **Categories Used:**
    * **Sports:** `rec.sport.baseball`, `rec.sport.hockey`
    * **Politics:** `talk.politics.guns`, `talk.politics.mideast`, `talk.politics.misc`.
* **Preprocessing:** Headers, footers, and quotes were stripped to ensure classification based purely on content.
  
# 🛠️ Techniques & Models
* **Feature Extraction:** CountVectorizer (Bag of Words)
* **Classifiers:**
    1.  Naive Bayes (Multinomial)
    2.  Logistic Regression
    3.  Linear Support Vector Machine (SVM)
    4.  Random Forest
    5.  K-Nearest Neighbors (KNN)

# 📊 Results Summary
The **Naive Bayes** achieved the highest accuracy, closely followed by Logistic Regression. KNN struggled with the high dimensionality of text data.

| Algorithm | Accuracy | F1-Score |
| :--- | :--- | :--- |
| Linear SVM | ~99.1% | ~0.99 |
| Logistic Regression | ~98% | ~0.99 |
| **Naive Bayes** | **~99.4%** | **~0.99** |
| Random Forest | ~98% | ~0.99 |
| KNN (k=5) | ~85% | ~0.88 |

# 🚀 How to Run
1.  **Install Dependencies:**
    ```bash
    pip install numpy pandas scikit-learn matplotlib
    ```
2.  **Run the Script:**
    ```bash
    python RollNumber_prob4.py
    ```
3.  **Output:**
    The script will print a comparison table to the console and save the detailed metrics to `model_comparison_results.csv`.

# 📝 Student Details
* **Assignment:** NLU Assignment 1
* **Problem:** 4 (Sports or Politics)
* **Roll Number:** M25MAC014
