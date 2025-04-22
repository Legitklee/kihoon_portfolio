---
title: "Ultrasonic Goalie Tabletop Game"
date: 2025-04-18
layout: post
categories: [projects]
---

**Timeline:** Jan 2025 – Present  
**Course Project:** Microprocessor-Based Mechanical Systems  
**Status:** In development

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
    <img src="https://via.placeholder.com/1000x500?text=Top+View+Placeholder" style="width: 100%;" alt="Slide 1">
    <img src="https://via.placeholder.com/1000x500?text=Block+Diagram+Placeholder" style="width: 100%;" alt="Slide 2">
    <img src="https://via.placeholder.com/1000x500?text=Prototype+Sketch+Placeholder" style="width: 100%;" alt="Slide 3">
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

The goal of this project is to create an interactive tabletop game that combines real-time sensing, control systems, and embedded electronics. The game simulates a mini soccer goal where a ball is rolled toward the goal, and a **servo-controlled goalie** dynamically moves to block it based on the detected ball position using **ultrasonic sensors**.

This project allows exploration of microprocessor integration, sensor fusion, and responsive actuation — all in a fun, real-world application.

---

### 🛠 Tools & Technologies

- **Microcontroller:** ESP32  
- **Sensors:** Two ultrasonic distance sensors (e.g. HC-SR04)  
- **Actuator:** Servo motor (e.g. SG90 or MG996R)  
- **Programming Language:** C++ via Arduino IDE or ESP-IDF  
- **Optional:** LabVIEW GUI for ball tracking and goal status  
- **Hardware:** Custom 3D-printed or laser-cut components

---

### 🚧 Planned Challenges & Goals

- Calibrating ultrasonic sensors for real-time ball tracking  
- Ensuring servo motor responds fast and accurately  
- Avoiding false readings and noise interference  
- Making the game fun, responsive, and replayable

---

### 🎯 Desired Outcome

- Ball tracking system using dual ultrasonic sensors  
- Goalie arm that intercepts ball based on predicted position  
- Visual/physical goal detection  
- (Optional) User interface for scoring and reset

---


