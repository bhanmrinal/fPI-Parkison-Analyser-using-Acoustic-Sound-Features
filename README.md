# fPI: Predicting Parkinson's with Acoustic Features

What is Parkinson's Disease?

Parkinson's disease is a neurodegenerative disorder that affects millions of people worldwide. It's characterized by the gradual loss of dopaminergic neurons in the brain, leading to tremors, rigidity, and difficulty with movement.

### Dataset
We've utilized a dataset containing biomedical voice measurements from 31 individuals. Here's a breakdown:

- Participants: 31 individuals (23 with Parkinson's, 8 healthy)\
- Format: Initially ASCII CSV, converted to .xlsx for easier analysis

 #### Attributes:
- Name: ``Subject name and recording number``

- Vocal Fundamental Frequency ``(MDVP:Fo, Fhi, Flo) ️``

- Jitter and Shimmer Measures ``(variation in frequency and amplitude)``

- Noise-to-Honer Ratio ``(NHR, HNR) ⚖️``

- Nonlinear Dynamical Complexity ``(RPDE, D2)``

- Signal Fractal Scaling Exponent ``(DFA)``

- Nonlinear Measures of Frequency Variation ``(spread1, spread2, PPE) 〰️``

- status: Health status ``(1 = Parkinson's, 0 = Healthy)``

### Novelty

Based on our correlation map analysis, we identified a potentially valuable feature combination: Denoted as the **fPI Analyser** 

``log10(DFA * D2 * spread2)``

- D2: Nonlinear dynamical complexity measure
- DFA: Signal fractal scaling exponent
- spread2: Nonlinear measure of fundamental frequency variation
This combined feature may offer stronger predictive power for Parkinson's detection using machine learning models.

### Model Development and Evaluation

We investigated the effectiveness of fPI by training and evaluating four machine learning models: **Decision Trees, Support Vector Machines, Random Forest, and XGBoost**. We used four performance metrics to assess their effectiveness: _Precision, Accuracy, F1-score, and Recall_. This comprehensive evaluation helped us identify the best model for Parkinson's detection using fPI.

### Deployment

This project is deployed as a full-stack web application, enabling global access to the Parkinson's disease detection system. The application leverages the following technologies:

``Frontend``: React.js for building dynamic and interactive user interfaces.

``Backend``: Django with Django REST framework (DRF) for rapid development of APIs and web applications. DRF provides a robust foundation for building RESTful APIs.

``Database``: PostgreSQL for storing and managing application data.

### Results 
<div align ="center">

![image](https://github.com/bhanmrinal/Predictive-Analysis-for-Parkinsons-Disease-using-ML/assets/97622240/037b3989-51b8-46d7-b163-6ea5af7ed9cd)

_Metric scores for different ML Models_

![image](https://github.com/bhanmrinal/Predictive-Analysis-for-Parkinsons-Disease-using-ML/assets/97622240/a114921b-c139-4809-a5e8-d2b7b9815b56)

_Metric plots for True Positive and False Positive Estimation_

 
</div>

