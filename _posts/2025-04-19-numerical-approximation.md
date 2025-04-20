---
title: "Numerical Approximation of Thermal Tile Thickness in Spacecraft Re-entry"
date: 2025-04-18
layout: post
categories: [projects]
---

**Timeline:** Spring 2023  
**Project Type:** Thermal Simulation & Numerical Analysis  
**Status:** Completed

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
    <img src="/portfolio/assets/images/num/img0.png" style="width: 100%;" alt="Slide 1">
    <img src="/portfolio/assets/images/num/img1.png" style="width: 100%;" alt="Slide 2">
    <img src="https://via.placeholder.com/1000x500?text=2D+Heat+Map+Placeholder" style="width: 100%;" alt="Slide 3">
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

Following the Columbia Shuttle Disaster, this project focused on the thermal protection system (TPS) tiles used during spacecraft atmospheric re-entry. The objective was to determine optimal tile thicknesses using 1D and 2D heat conduction simulations, applying various finite difference methods to solve Fourier’s heat equation and simulate thermal diffusion over time.

---

### 🛠 Tools & Numerical Methods Used

- **Platform:** MATLAB  
- **PDEs Solved:** 1D and 2D Fourier Heat Equation  
- **Numerical Methods:**  
  - Forward Differencing  
  - Leapfrog Method  
  - Dufort-Frankel  
  - Backward Differencing  
  - Crank-Nicolson (primary method used)  
- **GUI:** Built a simple MATLAB GUI to visualize simulation outcomes

---

### 📊 Simulation Design

- Evaluated multiple tiles with varying thickness under identical heat flux  
- Compared performance of different schemes based on stability, speed, and accuracy  
- Used Crank-Nicolson for its balance of **unconditional stability** and **second-order accuracy**  
- Extended simulation to model heat diffusion through tiles at different spatial grid resolutions

---

### 🚧 Challenges & Solutions

- **Numerical Stability:** Chose Crank-Nicolson after observing instability in explicit methods  
- **Convergence Speed:** Tuned time step size and node count for efficiency  
- **2D Modeling Complexity:** Required implementation of matrix-based thermal grid calculations

---

### ✅ Results & Impact

- Identified optimal TPS tile thickness for a given heat profile  
- Verified simulation results with analytical expectations  
- GUI enabled intuitive parameter tweaking for temperature and geometry  
- Highlighted value of simulation in early-stage spacecraft material planning

---

### 🔗 Report & Code

> You can view the full report and source code here:  
> [View on OneDrive](https://onedrive.live.com/view.aspx?resid=FDD192BF161FB1F6%213957&authkey=!AAvoj7YP1HN4d7I)

