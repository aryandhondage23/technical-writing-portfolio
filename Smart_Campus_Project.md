# AI-Enabled Smart Campus with Wireless Sensor Network

## Introduction

Electricity management is an important challenge
for colleges and universities. Sometimes lights,
fans and other electrical equipment remain switched
on even when classrooms are not being used.

This can lead to unnecessary electricity
consumption and increased costs.

To address this problem, we worked on an academic
research project called "AI-Enabled Smart Campus
with Wireless Sensor Network".

The main idea of this project is to combine
Wireless Sensor Networks (WSN) with Artificial
Intelligence to monitor electricity consumption
and identify unusual energy usage.

## What is the Main Idea?

The proposed system collects information such as
energy consumption, temperature and humidity.

This information can be analysed using machine
learning models to understand normal energy usage
and predict future consumption.

If actual energy consumption is significantly
different from the predicted value, the system
can identify it as a possible anomaly.

## Technologies Used

The proposed architecture includes:

- ESP8266 – Sensor node.
- PZEM-004T – Energy monitoring.
- DHT11 – Temperature and humidity monitoring.
- MQTT – Communication between sensor nodes
  and the gateway.
- Raspberry Pi 4 – Gateway.
- Python – Backend development and analysis.
- LSTM – Energy consumption forecasting.
- FastAPI – Backend API.
- Redis – Temporary storage and state management.
- SQLite – Storing logs and anomaly flags.

## How Does the System Work?

The proposed architecture has five main layers.

### 1. Sensing Layer

The sensing layer is designed to collect information
about electricity consumption and environmental
conditions using sensors.

### 2. Communication Layer

MQTT is used to transfer sensor information
from the sensor nodes to the gateway.

### 3. Gateway Layer

A Raspberry Pi 4 is proposed as the gateway.
It acts as a bridge between MQTT messages and
the backend system.

### 4. AI Analytics Layer

This is where machine learning is used.

An LSTM model analyses historical energy
consumption data and predicts future values.

The system compares actual consumption with
predicted consumption to identify unusual patterns.

### 5. Application Layer

The application layer stores information and
maintains anomaly flags using SQLite.

## Machine Learning Approach

We evaluated different forecasting approaches,
including:

- Linear Regression
- Random Forest
- XGBoost
- LSTM

Among the evaluated models, LSTM achieved the
best performance on the held-out test dataset.

The LSTM model achieved an R² score of 0.575
and reduced MAE by approximately 31% compared
with the persistence baseline.

We also explored an anomaly detection method
using hour-dependent thresholds.

This method achieved an average F1-score of
0.90 on the synthetic anomalies used in the study.

## My Learning Experience

Working on this project helped me understand how
Artificial Intelligence can be used to solve
practical problems.

I learned more about:

- Wireless Sensor Networks.
- Energy monitoring systems.
- Time-series data analysis.
- Machine learning and LSTM.
- Anomaly detection.
- Backend architecture.
- Technical research and documentation.

It also helped me understand the importance of
explaining technical ideas clearly through
research papers, diagrams and project reports.

## Current Limitations

One important point about our research is that
the physical Wireless Sensor Network has not
yet been deployed.

The sensor architecture is currently a design
specification.

The machine learning experiments were performed
using the UCI Appliances Energy Prediction
dataset as a proxy for classroom sensor data.

The anomaly detection experiments used synthetic
anomalies.

Testing the system with actual classroom sensor
data is part of our future work.

## Future Scope

In the future, we plan to:

- Deploy sensor nodes in actual classrooms.
- Collect real-time electricity consumption data.
- Improve prediction accuracy using real data.
- Test the anomaly detection system in real
  campus conditions.
- Explore additional features for smart energy
  management.

## Conclusion

This project gave me an opportunity to understand
how AI, sensors and data analysis can work together
to improve energy management.

It was a valuable learning experience because
I could connect theoretical concepts with a
practical problem.

It also improved my understanding of research,
technical documentation and teamwork.
