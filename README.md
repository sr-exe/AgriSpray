# 🌿 AgriSpray AI

<p align="center">
  Smart Pesticide Spraying System for Precision Agriculture

  FILES UPLOADINNG SOON
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Build-Vite-purple" />
  <img src="https://img.shields.io/badge/Frontend-React-blue" />
  <img src="https://img.shields.io/badge/Language-TypeScript-blue" />
  <img src="https://img.shields.io/badge/Style-TailwindCSS-38B2AC" />
  <img src="https://img.shields.io/badge/Status-Active-success" />
</p>

---

## 📌 About

AgriSpray AI is a smart pesticide spraying system interface built for **precision agriculture**. It helps users capture live leaf images, analyze visible symptoms, and review scan analytics through a modern web dashboard.

The project focuses on **reducing unnecessary pesticide usage** by supporting **targeted decisions instead of blanket spraying**.

---

## 🚀 Overview

This application provides:

✨ live camera-based leaf capture  
✨ on-device visual symptom screening  
✨ scan history with real-time analytics  
✨ weekly reporting and disease distribution charts  
✨ system flow and technology overview pages  
✨ responsive UI with light and dark mode  

---

## ✨ Key Features

### 📷 Live Detection
Opens the device camera, captures a leaf frame, validates image quality, and checks for visible symptoms.

### 🧠 Smart Validation
Rejects scans when:
- no clear leaf is detected  
- frame is too dark  
- blurry image  
- overexposed capture  

### 📊 Real-Time Analytics
Stores valid scans locally and updates dashboard numbers and charts from real scan history.

### 🎨 Interactive UI
Includes:
- smooth animations  
- themed navigation  
- polished cards  
- tab-based analytics views  

### 🌗 Theme Support
Users can switch between **light and dark mode**.

---

## 🔄 System Flow

The intended workflow is:

```mermaid
graph TD
A[Capture Leaf Image] --> B[Validate Image Quality]
B --> C[Analyze Color & Stress]
C --> D{Symptoms Present?}
D -->|Yes| E[Trigger Spray Logic]
D -->|No| F[Reject / No Action]
E --> G[Save to Analytics]
F --> G

```

### 👨‍💻 Contributors
- SHUBHAM RATHOD
- SHAIKH RIZWAN
