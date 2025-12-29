# BMS / SCADA Energy Anomaly & Failure Risk Detection

## Overview
Large buildings and infrastructure facilities rely on Building Management
Systems (BMS) and SCADA platforms to monitor and control critical equipment
such as chillers, air handling units (AHUs), pumps, and electrical systems.

Abnormal system behavior can result in:
- Excessive energy consumption
- Accelerated equipment wear
- Comfort and safety issues
- Unexpected equipment failure

This project demonstrates how machine learning can be used as a
**decision-support tool** to:
- Detect anomalous operational behavior
- Estimate relative equipment failure risk

The emphasis is on **interpretability, operational relevance,
and responsible use of ML**, rather than black-box automation.

---

## Problem Statement
BMS / SCADA systems generate large volumes of sensor and operational data.
However, identifying early warning signs of equipment degradation
remains challenging in complex facilities.

This project addresses two key maintenance questions:
1. *Is the equipment operating abnormally?*
2. *If abnormal behavior is detected, how risky is the situation?*

By separating anomaly detection from failure risk estimation,
the project mirrors real-world preventive maintenance workflows.

---

## Data Strategy
Due to the sensitive and proprietary nature of real BMS / SCADA data,
a **synthetic dataset** is generated to simulate realistic operational conditions.

The dataset includes:
- Equipment type (Chiller, AHU, Pump)
- Average operating temperature
- Power consumption
- Runtime hours per day
- Load percentage
- Alarm frequency
- Days since last maintenance
- Anomaly indicator
- Failure risk score

Synthetic data generation allows transparent modeling of
cause–effect relationships while avoiding the use of confidential data.

---

## Exploratory Data Analysis (EDA)
EDA focuses on identifying early warning signals and degradation patterns,
including:
- Elevated temperature and power consumption
- Increased runtime and sustained high load
- Frequent alarms and delayed maintenance
- Correlation between anomalies and rising failure risk

The analysis prioritizes **maintenance-relevant insights**
over exhaustive visualization.

---

## Modeling Approach
Two simple and interpretable models are used:

- **Logistic Regression** for anomaly detection
- **Linear Regression** for failure risk estimation

These models are intentionally selected to:
- Ensure transparency and explainability
- Support trust among maintenance and facilities teams
- Avoid black-box decision-making in safety- and reliability-critical systems

---

## Evaluation
Model evaluation emphasizes practical usefulness:
- Classification metrics and confusion matrix for anomaly detection
- MAE and RMSE for failure risk estimation

In BMS / SCADA environments, missing an early warning signal
is often more costly than triggering a false alarm.

---

## Limitations & Ethical Considerations
- The dataset is synthetic and based on assumed system behavior.
- Real-world systems may exhibit sensor noise, communication delays,
  and unexpected operational patterns.
- Model outputs should not be used as the sole basis
  for maintenance or safety decisions.

Machine learning is positioned as a **support tool for engineers**,
not as a replacement for human judgment.

---

## Conclusion
This project illustrates how machine learning can be applied responsibly
to anomaly detection and failure risk estimation in BMS / SCADA systems.

By emphasizing interpretability, early warning signals,
and operational relevance, the project highlights the role of ML
in preventive maintenance and energy-efficient facility operations.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn


## Author
Sandesh Duduskar
