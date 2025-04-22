---
title: "Diabetes Classifier"
date: 2025-04-18
layout: post
categories: [projects]
---

**Timeline:** Fall 2024  
**Project Type:** ML Project  

---

<!-- Image Carousel -->
<div class="glider-contain" style="position: relative; width: 100%; overflow: hidden; margin: 2rem 0;">
  <button aria-label="Previous" class="glider-prev" style="
    position: absolute;
    top: 50%;
    left: 10px;
    z-index: 10;
    background-color: rgba(0,0,0,0.5);
    color: white;
    border: none;
    font-size: 2rem;
    transform: translateY(-50%);
    padding: 0.5rem 1rem;
    cursor: pointer;
  ">❮</button>

  <button aria-label="Next" class="glider-next" style="
    position: absolute;
    top: 50%;
    right: 10px;
    z-index: 10;
    background-color: rgba(0,0,0,0.5);
    color: white;
    border: none;
    font-size: 2rem;
    transform: translateY(-50%);
    padding: 0.5rem 1rem;
    cursor: pointer;
  ">❯</button>

  <div class="glider">
    <img src="https://via.placeholder.com/1000x500?text=ROC+Curve+Placeholder" style="width: 100%;" alt="Slide 1">
    <img src="https://via.placeholder.com/1000x500?text=Confusion+Matrix+Placeholder" style="width: 100%;" alt="Slide 2">
    <img src="https://via.placeholder.com/1000x500?text=Feature+Importance+Placeholder" style="width: 100%;" alt="Slide 3">
  </div>

  <div role="tablist" class="dots" style="text-align: center; margin-top: 1rem;"></div>
</div>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/glider-js@1/glider.min.css">
<script src="https://cdn.jsdelivr.net/npm/glider-js@1/glider.min.js"></script>
<script>
  window.addEventListener('load', function(){
    new Glider(document.querySelector('.glider'), {
      slidesToShow: 1,
      dots: '.dots',
      arrows: {
        prev: '.glider-prev',
        next: '.glider-next'
      }
    });
  });
</script>

---

### 🧩 Problem Statement

This project aimed to develop a machine learning model capable of classifying whether a person is likely to have diabetes based on medical attributes. It was built to explore the practical application of supervised classification models in healthcare using structured health datasets.

---

### 🛠 Tools & Techniques

- **Language:** Python  
- **Libraries:** Pandas, Scikit-learn, TensorFlow, Keras, Matplotlib  
- **Models Used:** Logistic Regression, Decision Tree, Random Forest, Support Vector Machine, Neural Network  
- **Evaluation Metrics:** Accuracy, Precision, Recall, ROC AUC

---

### 📊 Dataset

- **Source:** PIMA Indian Diabetes Dataset (UCI / Kaggle)  
- 768 samples with 8 features each  
- Features: Glucose level, BMI, Age, Insulin, Pregnancies, Blood Pressure, etc.  
- Target: Binary outcome (diabetic vs non-diabetic)

---

### 🚧 Challenges & Insights

- **Imbalanced Classes:** Required metric tuning beyond accuracy  
- **Missing Values:** Some features (like insulin) had missing or zero-like values  
- **Feature Scaling:** Critical for neural network convergence  
- **Model Selection:** Random Forest and Neural Network performed best overall

---

### ✅ Results & Impact

- Achieved **~85% accuracy** and strong performance on ROC curve  
- Neural network with ReLU activation and dropout produced stable results  
- Improved understanding of the trade-offs between model interpretability and performance  
- Future iterations could integrate with a frontend for clinical screening demos

