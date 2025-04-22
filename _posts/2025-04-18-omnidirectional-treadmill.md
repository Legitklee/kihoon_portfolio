---
title: "Omnidirectional Treadmill"
date: 2025-04-18
layout: post
categories: [projects]
image: /assets/images/treadmill-diagram.png
---

**Timeline:** Sep 2024 – Present  
**Project Type:** UC Berkeley M.Eng Capstone  
**Partner:** Blue Goji (Gamified Fitness Company)

---

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
    <img src="/portfolio/assets/images/omni/img2.png" style="width: 100%;" alt="Slide 1">
    <img src="/portfolio/assets/images/omni/img0.png" style="width: 100%;" alt="Slide 2">
    <img src="/portfolio/assets/images/omni/img1.png" style="width: 100%;" alt="Slide 3">
  </div>

  <div role="tablist" class="dots" style="text-align: center; margin-top: 1rem;"></div>
</div>


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

Traditional treadmills allow only linear forward motion, limiting their effectiveness in replicating natural, complex human movement. Our goal was to design an omnidirectional treadmill that enables free movement in any direction **without using motors**, making it **cost-effective**, intuitive, and suitable for **rehabilitation, VR, and military training**.

---

### 🔧 Approach & Process

We developed a resistive omnidirectional treadmill that:
- Uses a **center plate** with **freely rotatable ball rollers** for smooth multi-directional sliding
- Surrounds the center with angled plates that guide the user back to center using **gravity**
- Incorporates **two braking systems**:
  - **Magnetic braking** for precise control in the center zone using electromagnetic current
  - **Friction braking** on angled plates using lift-controlled rubber contact to save cost

This hybrid approach allowed us to maintain user control while minimizing complexity and price.

---

### ⚙️ Tools & Methods Used
- CAD design in **SolidWorks**
- Simulation & analysis via **FEA**
- Prototyping with scaled 3D models
- Cost-performance optimization using component trade-off matrices

---

### 🚧 Challenges & Solutions

- **Motorless movement control:** Solved using electromagnets and gravity-inclined plates  
- **Cost constraints:** Replaced motor systems with friction braking where precision was less critical  
- **User intuitiveness:** Designed a layout that naturally guides users toward the center

---

### ✅ Results & Impact

- Developed a **fully functional prototype** capable of multi-directional user movement
- Reduced cost by ~40% compared to motorized treadmill systems
- Collaborated with **Blue Goji** to explore future applications in gamified rehab and VR

---


<!-- Glider.js CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/glider-js@1/glider.min.css">

<!-- Glider.js script -->
<script src="https://cdn.jsdelivr.net/npm/glider-js@1/glider.min.js"></script>
