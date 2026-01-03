## Problem Statement

In many educational institutions, students experience a gradual decline in academic performance due to factors such as poor attendance, insufficient study hours, low engagement, and lack of timely academic guidance. Conventional evaluation systems identify academic failure only after final examinations, leaving no opportunity for early intervention.

There is a strong need for an intelligent system that can predict academic risk at an early stage using Machine Learning and provide personalized, actionable guidance using Generative AI, enabling students to take corrective measures proactively and improve learning outcomes.

## Proposed Solution

This project presents a hybrid Machine Learning + Generative AI system that acts as an early-warning academic mentor.

The system:

Predicts student academic risk levels (High / Medium / Low) using a supervised ML model.

Explains predictions using model confidence and feature importance.

Generates personalized improvement guidance using a Large Language Model (LLM).

The solution bridges the gap between raw ML predictions and human-understandable academic support.

## Objectives

Predict student academic risk before final examinations.

Enable early academic intervention.

Provide explainable and transparent ML predictions.

Deliver personalized learning guidance using Generative AI.

Demonstrate practical integration of ML + AI in education.

## System Architecture
Student Academic Data
        ↓
Machine Learning Model
        ↓
Risk Prediction (High / Medium / Low)
        ↓
Model Confidence & Feature Importance
        ↓
Generative AI Mentor
        ↓
Personalized Improvement Guidance

## Dataset

Student Performance Dataset (Kaggle)
🔗 https://www.kaggle.com/datasets/devansodariya/student-performance-data

Dataset Features:

Attendance percentage

Study hours

Assignment scores

Participation level

Midterm and final scores

## Technology Stack
Component	Technology
Programming Language	Python
Machine Learning	scikit-learn
Explainability	SHAP
Generative AI	Google Gemini API
Development Environment	Google Colab
Data Processing	Pandas, NumPy
## Machine Learning Approach

Problem Type: Multiclass Classification

Model Used: Random Forest Classifier

Target Variable: Academic Risk Level

Evaluation Metrics:

Accuracy

Precision

Recall

F1-Score

The model classifies students into High, Medium, or Low academic risk categories based on academic indicators.

## Generative AI Component

The AI Mentor module converts ML outputs into student-friendly explanations and recommendations.

Responsibilities:

Explain predicted risk levels in simple language.

Provide exactly three personalized improvement suggestions.

Maintain supportive and motivational tone.

Never alter ML predictions.

 ## Security & Ethics:

API keys are managed using environment variables.

No API keys are stored in code or repositories.

AI responses are grounded in ML outputs to prevent hallucination.
