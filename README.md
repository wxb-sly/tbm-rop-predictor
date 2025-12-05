# Iron Mole: TBM Performance & Risk Prediction Engine

> **Mission:** To translate geotechnical uncertainty into quantifiable schedule risk, enabling infrastructure owners to preempt cost overruns in high-capital tunneling projects.

### 1. The Problem (The Liability)
Tunnel Boring Machines (TBMs) are $100M+ assets operating in blind, high-entropy environments. A purely deterministic schedule ("We will average 15m/day") fails to account for geological non-linearity (e.g., massive granite or squeezing ground).
**The Commercial Consequence:** Unexpected deceleration leads to cascading delays, Liquidated Damages (LDs), and potential insolvency.

### 2. The Solution (The Method)
This engine deploys **Gradient Boosted Decision Trees (XGBoost)** to model the non-linear interaction between Machine Parameters (Thrust, RPM) and Geological Reality (UCS, RQD). Unlike traditional linear regression, it captures the "stall points" where rock strength overwhelms machine power.
*   **Physics-Informed Data Synthesis:** Simulates CSM (Colorado School of Mines) rock-cutting mechanics.
*   **Predictive Modeling:** XGBoost Regressor for Rate of Penetration (ROP).
*   **Explainable AI (XAI):** SHAP (Shapley Additive exPlanations) to audit *why* the model predicts a slowdown.

### 3. The Result (The Asset)
A deployable risk model that provides:
*   **Precision Forecasting:** ROP predictions with <10% RMSE.
*   **Risk Quantification:** Early warning of "Red Zones" (ROP < 1.0 m/hr) prior to excavation.
*   **Capital Protection:** Data-backed justification for contingency fund allocation and schedule renegotiation.

---
**Tech Stack:** Python, XGBoost, SHAP, Scikit-Learn, Pandas.
**Status:** [Active Development]
