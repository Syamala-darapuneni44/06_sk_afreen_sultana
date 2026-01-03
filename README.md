
##  Problem Statement

In many educational institutions, students experience a gradual decline in academic performance due to factors such as poor attendance, insufficient study hours, low engagement, and lack of timely academic guidance. Conventional evaluation systems often identify academic failure only after final examinations, leaving no opportunity for early intervention.

There is a strong need for an intelligent system that can **predict academic risk at an early stage using Machine Learning** and **provide personalized, actionable guidance using Large Language Models (LLMs) and Agent-based AI**, enabling students to take corrective measures proactively and improve learning outcomes.



##  Proposed Solution

This project presents a **hybrid Machine Learning + Generative AI + Agentic AI system** that acts as an **early-warning academic mentor**.

The system:

* Predicts student academic risk levels (**High / Medium / Low**) using a supervised Machine Learning model.
* Explains predictions using model confidence and feature importance for transparency.
* Uses a **Large Language Model (LLM)** to convert predictions into human-friendly explanations.
* Employs an **agent-based AI (LangChain Agent)** to reason over student data and generate **personalized, structured academic guidance**.

This approach bridges the gap between raw ML predictions and **actionable, student-centered academic mentorship**.



##  Objectives

* Predict student academic risk before final examinations.
* Enable early and preventive academic intervention.
* Provide explainable and transparent ML predictions.
* Deliver personalized learning guidance using **LLMs and Agent-based AI**.
* Demonstrate practical, real-world integration of **Machine Learning, LLMs, and Agentic AI** in education.



##  System Architecture

```
Student Academic Data
        ↓
Machine Learning Model (Random Forest)
        ↓
Risk Prediction (High / Medium / Low)
        ↓
Model Confidence & Feature Importance (SHAP)
        ↓
Agent-based AI (LangChain Agent)
        ↓
Large Language Model (LLM)
        ↓
Personalized Improvement Guidance
```


## Dataset

**Student Performance Dataset (Kaggle)**
🔗 [https://www.kaggle.com/datasets/devansodariya/student-performance-data](https://www.kaggle.com/datasets/devansodariya/student-performance-data)

### Dataset Features:

* Attendance percentage
* Study hours
* Assignment scores
* Participation level
* Midterm and final examination scores

Each record represents an individual student, making the dataset suitable for supervised learning and early academic risk analysis.



##  Technology Stack

| Component               | Technology                            |
| ----------------------- | ------------------------------------- |
| Programming Language    | Python                                |
| Machine Learning        | scikit-learn                          |
| Explainability          | SHAP                                  |
| Generative AI / LLM     | Google Gemini API / Groq-hosted LLaMA |
| Agent Framework         | LangChain                             |
| Development Environment | Google Colab                          |
| Data Processing         | Pandas, NumPy                         |



##  Machine Learning Approach

* **Problem Type:** Multiclass Classification
* **Model Used:** Random Forest Classifier
* **Target Variable:** Academic Risk Level (High / Medium / Low)
* **Evaluation Metrics:**

  * Accuracy
  * Precision
  * Recall
  * F1-Score

The ML model learns patterns from academic and behavioral features to classify students into appropriate risk categories.



## Generative AI & Agent-Based Component

The **AI Mentor module** enhances the ML predictions by integrating **LLMs and Agentic AI**.

### Key Responsibilities:

* Explain predicted risk levels in simple, non-technical language.
* Reason over student data using an **AI agent** rather than a simple chatbot.
* Provide **exactly three personalized improvement recommendations**.
* Maintain a supportive and motivational tone.
* Ensure AI outputs are **grounded in ML predictions** and do not alter model decisions.

The LangChain agent follows a **Reason–Act pattern**, selecting the appropriate mentoring logic before generating responses using the LLM.



##  Security & Ethics

* API keys are securely managed using **environment variables / Colab Secrets**.
* No API keys are stored in code or pushed to repositories.
* The AI system does **not override or modify ML predictions**.
* AI responses are grounded in structured ML outputs to prevent hallucination.
* The system promotes transparency, fairness, and responsible AI usage in education.

