---
title: "Jar Opening Device"
date: 2025-04-18
layout: post
categories: [projects]
---

**Timeline:** Spring 2024  
**Project Type:** Product Design Engineering  
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
    <img src="/portfolio/assets/images/jar/img0.png" style="width: 100%;" alt="Slide 1">
    <img src="/portfolio/assets/images/jar/img1.png" style="width: 100%;" alt="Slide 2">
    <img src="/portfolio/assets/images/jar/img2.png" style="width: 100%;" alt="Slide 3">
    <img src="/portfolio/assets/images/jar/img3.png" style="width: 100%;" alt="Slide 4">
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

The project focused on creating an assistive device for individuals with arthritis or reduced hand strength who struggle with opening jars. The objective was to **reduce the torque** required while ensuring **comfort, usability, and safety** — all while remaining low-cost and easy to manufacture.

---

### 🛠 Tools & Methods Used

- **Design Process:** User research, product specification, ergonomic studies  
- **Concept Development:** Brainstorming, sketching, prototyping  
- **Evaluation:** Pugh’s Matrix for concept selection  
- **CAD Modeling:** Autodesk Inventor  
- **Material + Manufacturing Review:** Stress vs. grip material selection, cost vs. recyclability

---

### ⚙️ Design Highlights

- Generated multiple design concepts ranging from simple mechanical arms to compound-grip systems  
- Evaluated designs using a **weighted decision matrix**  
- Final design chosen for balance of mechanical advantage, cost, and ease of use  
- CAD model optimized for 3D printing or injection molding

---

### 🚧 Challenges & Solutions

- **User comfort vs. torque delivery:** Balanced gear-based and lever-style solutions  
- **Manufacturing method:** Considered injection molding vs. manual assembly trade-offs  
- **Designing for grip variance:** Included adjustable components for different jar sizes

---

### ✅ Results & Impact

- Final CAD model delivered and validated with simulated torque reduction  
- Focused on simplicity and intuitive operation for aging users  
- Ready for prototyping and pilot testing in accessibility-focused product pipelines

