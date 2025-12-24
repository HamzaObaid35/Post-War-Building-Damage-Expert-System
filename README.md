# Building Damage Assessment Expert System

An expert system designed to assess building damage after war or natural disasters using a hybrid approach that combines **Fuzzy Logic** and **Probabilistic Reasoning (Bayesian Networks)**.

## 📖 Overview
Assessing building damage after conflicts or disasters is complex due to uncertainty, imprecise data, and multiple interacting damage factors. Traditional manual inspections are time-consuming and subjective.

This project proposes an **automated expert system** that evaluates building damage severity by integrating:
- Fuzzy Logic to handle imprecise inputs
- Bayesian Networks to model dependencies and probabilities

The system outputs a **final damage score and classification**:
- Minor Damage
- Moderate Damage
- Severe Damage

## 🧠 System Methodology

### 1. Fuzzy Logic Module
Handles uncertain and imprecise inputs using membership functions.

**Input Variables:**
- Crack Width
- Leaning Angle
- Roof Sagging
- Foundation Cracks
- Fire Level

**Output:**
- Damage Severity Score (0–10)

Damage Classification:
- 0 – 4 → Minor
- 4 – 8 → Moderate
- 8 – 10 → Severe

### 2. Probabilistic Reasoning (Bayesian Network)
Models dependencies between damage factors and estimates damage probabilities.

**Key Features:**
- Nodes represent damage factors
- Conditional Probability Distributions (CPDs)
- Variable Elimination for inference

**Output:**
- Probability of each damage level
- Most likely damage category

### 3. Hybrid Integration
The final damage score is computed using a **weighted average**:
- 50% Fuzzy Logic result
- 50% Bayesian Network result

## 📊 Example Input & Output

**Sample Inputs:**
- Crack Width: 4 mm
- Leaning Angle: 1.5%
- Roof Sagging: 6 cm
- Foundation Cracks: 7 mm
- Fire Level: 50%

**Results:**
- Fuzzy Score: 5.53
- Bayesian Result: Moderate Damage (60%)
- Final Score: 6.77
- Final Classification: **Moderate Damage**

## 🗂 Project Structure

```text
├── Building_Damage_Expert_System_Code.ipynb
├── Building_Damage_Assessment_Report.pdf
├── Building_Damage_Knowledge_Base.pdf
├── Expert_System_Approach_Presentation.pptx
└── README.md
