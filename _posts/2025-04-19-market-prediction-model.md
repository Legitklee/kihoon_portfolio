---
title: "Market Prediction Model"
date: 2025-04-18
layout: post
categories: [projects]
---

**Timeline:** Fall 2024  
**Personal ML Project**  

---

<!-- Carousel Starts Here -->
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
    <img src="https://via.placeholder.com/1000x500?text=Feature+Importance+Plot" style="width: 100%;" alt="Slide 1">
    <img src="https://via.placeholder.com/1000x500?text=Prediction+vs+True+Value+Graph" style="width: 100%;" alt="Slide 2">
    <img src="https://via.placeholder.com/1000x500?text=Data+Distribution+Visualization" style="width: 100%;" alt="Slide 3">
  </div>

  <div role="tablist" class="dots" style="text-align: center; margin-top: 1rem;"></div>
</div>

<!-- Glider.js -->
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

This project aimed to estimate the **market value of professional soccer players** using machine learning. Inspired by real-world transfer market dynamics, the model was built to analyze patterns in player stats and characteristics, and output a predicted market value — a valuable asset for clubs, analysts, or scouting platforms.

---

### 🛠 Tools & Technologies

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib  
- **Algorithms:** Linear Regression, Ridge Regression, Decision Tree, Random Forest  
- **Preprocessing:** One-hot encoding for categorical features, normalization for numerical data  
- **Evaluation Metrics:** R² Score, RMSE

---

### 📊 Dataset

- **Source:** Public Kaggle dataset on FIFA/Transfermarkt player stats  
- ~10,000 player samples  
- Features included: age, nationality, position, rating, goals, assists, minutes played, and more  
- Output: Player market value in USD (continuous target)

---

### 🚧 Challenges & Insights

- **Data imbalance** — many players had low market values, few had extreme highs  
- **Feature selection** — model performance improved by dropping noisy or overly correlated fields  
- **Model tuning** — Ridge regression + decision trees gave the best trade-off between bias and variance  
- **Interpretability** — found player position, age, and minutes played were the most influential features

---

### ✅ Results & Impact

- Achieved **R² score of 0.81** on test set  
- Model effectively captured value trends across player demographics and performance  
- Can be extended into web dashboards or integrated into scouting systems  
- Reinforced understanding of end-to-end ML pipelines: from raw data to predictions and evaluation

---
