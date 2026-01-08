# Architecture Layers

EcoSync Lite is structured into four conceptual layers to ensure clarity, scalability, and safety.

## 1. Data Acquisition Layer
This layer is responsible for collecting time-series data such as:
- Indoor environmental conditions
- Occupancy indicators
- Electrical load measurements
- Operational state signals

The layer supports both live sensor input and synthetic or simulated data.

## 2. Edge Processing Layer
The edge gateway performs:
- Data preprocessing and normalization
- Anomaly filtering
- Short-term forecasting (conceptual)
- Enforcement of deterministic safety rules

All critical decisions occur locally within this layer.

## 3. Decision and Control Layer
Based on processed data, the system determines whether energy-consuming loads can be safely reduced, deferred, or maintained without violating comfort or operational constraints.

## 4. Verification and Reporting Layer
This layer records:
- Energy consumption changes
- Control actions taken
- Comfort compliance
- Estimated environmental impact

These layers operate cohesively but remain logically separable.

