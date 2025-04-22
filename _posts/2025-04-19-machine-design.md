---
title: "Machine Design"
date: 2025-04-18
layout: post
categories: [projects]
---

**Timeline:** Fall 2023  
**Project Type:** Mechanical Design Engineering  
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
    <img src="/portfolio/assets/images/machine/img0.png" style="width: 100%;" alt="Slide 1">
    <img src="/portfolio/assets/images/machine/img1.png" style="width: 100%;" alt="Slide 2">
    <img src="/portfolio/assets/images/machine/img2.png" style="width: 100%;" alt="Slide 3">
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

This project aimed to design a sustainable machine and supply chain system for converting **shredded carbon fiber waste** into **eco bricks** for construction and reuse. The challenge was to develop a low-energy, high-throughput system that maximized output while minimizing energy cost and failure modes.

---

### 🛠 Tools & Methods Used

- **CAD Software:** Autodesk Inventor  
- **Failure Analysis:** UML Diagrams, FMECA, Fault Tree Analysis  
- **Design Evaluation:** Pugh’s Matrix  
- **Component Selection:** Sensor logic, material stress calculations, conveyor layouts

---

### ⚙️ Design Process

- Generated four initial design concepts for the recycling and production process  
- Used **Pugh’s matrix** to evaluate designs against production cost, energy usage, and scalability  
- Developed a track-based system for material flow, using gravity-assisted drop zones  
- Designed custom brackets, friction interfaces, and molds for brick forming  
- Conducted reliability and safety analysis for supply chain elements

---

### 🚧 Challenges & Solutions

- **Outsourcing vs. Manufacturability:** Metal connector design would’ve required expensive outsourcing; instead, we created simplified in-house fabricatable components  
- **Reliability Tracking:** Used UML and FMECA diagrams to detect failure points early  
- **Energy Optimization:** Introduced slope-based material handling to reduce energy draw from actuators

---

### ✅ Results & Impact

- Delivered a final system that met **production and energy requirements**  
- Reduced overall energy consumption per eco brick with gravity-fed material movement  
- Produced a design ready for small-scale prototyping or pilot manufacturing  
- Surpassed investor expectations for energy efficiency and throughput rate

