# Building Damage Assessment Expert System

An intelligent expert system for assessing building damage after war or natural disasters using a hybrid approach that combines **Fuzzy Logic** and **Bayesian Networks** to handle uncertainty and complex damage interactions.

---

## 📖 Overview

Assessing building damage in post-war or disaster scenarios is a challenging process due to incomplete information, uncertainty, and the interaction of multiple damage factors such as structural cracks, leaning, roof sagging, foundation damage, and fire exposure. Traditional assessment methods rely heavily on manual inspections, which are time-consuming, subjective, and prone to human error.

This project presents an **automated expert system** designed to evaluate building damage severity accurately by integrating fuzzy logic with probabilistic reasoning. The system provides a final damage score and classifies the building condition into **Minor**, **Moderate**, or **Severe** damage levels.

---

## 🎯 Objectives

- Automate the building damage assessment process  
- Handle imprecise and uncertain input data effectively  
- Reduce reliance on manual inspections  
- Support decision-making in post-war reconstruction and disaster recovery  

---

## 🧠 System Architecture

The expert system consists of three main components:

### 1️⃣ Fuzzy Logic Module

Handles vague and imprecise input values using membership functions and fuzzy rules.

**Input Variables:**
- Crack Width  
- Leaning Angle  
- Roof Sagging  
- Foundation Cracks  
- Fire Level  

**Output:**
- Damage Severity Score (0–10)

**Damage Classification:**
- 0 – 4 → Minor Damage  
- 4 – 8 → Moderate Damage  
- 8 – 10 → Severe Damage  

---

### 2️⃣ Probabilistic Reasoning Module (Bayesian Network)

Models probabilistic relationships and dependencies between damage factors.

**Key Features:**
- Nodes represent damage indicators  
- Conditional Probability Distributions (CPDs)  
- Probabilistic inference using Variable Elimination  

**Output:**
- Probability distribution of damage levels  
- Most likely damage classification  

---

### 3️⃣ Hybrid Integration Approach

The final damage score is calculated using a **weighted average**:
- 50% from the Fuzzy Logic output  
- 50% from the Bayesian Network output  

This hybrid approach improves robustness and reliability in uncertain environments.

---

## 📊 Example Assessment

**Sample Inputs:**
- Crack Width: 4 mm  
- Leaning Angle: 1.5%  
- Roof Sagging: 6 cm  
- Foundation Cracks: 7 mm  
- Fire Level: 50%  

**Results:**
- Fuzzy Logic Score: 5.53  
- Bayesian Result: Moderate Damage (60%)  
- Final Combined Score: 6.77  
- Final Damage Level: **Moderate Damage**

---

## 🗂 Project Structure

```text
Building-Damage-Assessment-Expert-System/
│
├── Building_Damage_Expert_System_Code.ipynb
├── Building_Damage_Assessment_Report.pdf
├── Building_Damage_Knowledge_Base.pdf
├── Expert_System_Approach_Presentation.pptx
└── README.md
