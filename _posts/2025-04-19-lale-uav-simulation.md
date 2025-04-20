---
title: "LALE Solar UAV Simulation and Flight Optimization"
date: 2025-04-18
layout: post
categories: [projects]
---

**Timeline:** Jan 2023 – May 2023  
**Partner:** Limosaero  
**Project Type:** Undergraduate Engineering Research  

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
    <img src="/portfolio/assets/images/uav/img0.png" style="width: 100%;" alt="Slide 1">
    <img src="https://via.placeholder.com/1000x500?text=Solar+Input+Graph+Placeholder" style="width: 100%;" alt="Slide 2">
    <img src="https://via.placeholder.com/1000x500?text=Cloud+Map+Coverage+Placeholder" style="width: 100%;" alt="Slide 3">
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

The objective of this simulation was to identify how cloud coverage, solar irradiance, and flight strategies impact the **range and time-in-air** of a solar-powered UAV. Working with Limosaero, the project aimed to develop a code-based flight model with two degrees of freedom and optimize performance based on **latitude, time of year, and solar conditions**.

---

### 🛠 Tools & Methods Used

- **Environment:** MATLAB  
- **Input Data:** Solar irradiance code, BBC Weather satellite imagery  
- **Modeling:** UAV trajectory simulation under varying solar and atmospheric conditions  
- **Post-Processing:** Battery level estimation, power input/output curves, solar intensity heatmaps

---

### 📊 Strategy & Dataset Modeling

- Solar irradiance values were calculated based on **time of day and date**, simulating **summer solstice, equinox, and winter solstice** at a fixed location.
- Cloud coverage images were parsed pixel-by-pixel and assigned **intensity coefficients**, simulating power loss from cloud occlusion.
- The UAV's **power consumption** was computed via drag force calculations for different speeds and flight paths.

---

### 🚧 Challenges & Insights

- **Energy Input vs. Drag Tradeoff**: Maintaining minimum drag speed was energy-efficient but reduced range  
- **Time of Flight Impact**: Modifying trajectory in early morning hours (4–5am) significantly boosted range  
- **Cloud mapping**: Accurately modeling real cloud cover from visual maps improved result realism

---

### ✅ Results & Impact

- Optimized trajectory during summer solstice increased UAV range by **313 km**
- Minimum drag velocity: **12 m/s**; Optimal summer strategy: **21 m/s with adjusted path**
- Morning trajectory modifications between **4–5am** yielded best range across all seasons
- Identified **90Wh energy savings** with modified winter trajectory between **9am–2pm**

---

### 🌱 Future Potential

- Integrating **latitude** and **wind data** for global flight strategy  
- Adding **moving cloud systems** and terrain effects  
- Extending model to optimize **battery health** and **real-time rerouting**

