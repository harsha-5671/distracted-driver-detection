# Distracted Driver Detection – Machine Learning Project

## 1. Problem Statement
Distracted driving is a major cause of road accidents worldwide. Activities such as using a mobile phone, talking to passengers, or adjusting in-car controls divert the driver’s attention from the road and significantly increase accident risk.

The objective of this project is to **detect distracted driving behavior from images captured by an in-car camera** using a machine learning approach. Given an image of a driver, the system predicts the driver’s activity class.

---

## 2. Why Machine Learning?
Rule-based approaches are not suitable for this problem because:

- Drivers differ in appearance, posture, and behavior
- Lighting conditions vary (day/night, shadows)
- Camera angles and backgrounds are inconsistent
- Visual cues such as hand position and head orientation are complex

A **data-driven machine learning model** can learn these visual patterns directly from image data and generalize better to unseen driving scenarios.

---

## 3. Problem Type
- **Learning Type:** Supervised Learning  
- **Task:** Image Classification  
- **Classification Type:** Multi-class classification  

Each input image belongs to exactly one driver behavior class.

---

## 4. Input and Output Definition

### Input
- A single RGB image of a driver
- Image captured from an in-car camera
- Images will be resized and normalized during preprocessing

### Output
- A predicted driver behavior class (e.g., safe driving, texting, talking, etc.)
- Probability scores will be used during evaluation

---

## 5. Dataset (High-Level Overview)
- **Source:** Kaggle (State Farm Distracted Driver Detection dataset)
- **Data Type:** Images
- **Classes:** Multiple driver behavior categories

Detailed dataset analysis and class distribution will be documented separately in the `data/` directory.

---

## 6. Evaluation Criteria
Model performance will be evaluated using:
- Overall accuracy
- Class-wise precision and recall
- Confusion matrix

Since this is a **safety-critical problem**, special emphasis will be placed on **recall for distracted driving classes**, as missing a distracted driver is more critical than false positives.

---

## 7. Project Scope (Phase 1)
This phase of the project focuses on building a **standalone machine learning pipeline**, including:
- Dataset understanding and exploration
- Model design and training
- Evaluation and analysis

Backend APIs, frontend UI, and deployment will be added in later phases without modifying the core ML logic.
