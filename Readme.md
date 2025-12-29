# Aircraft Trajectory Prediction Using LSTM ✈️

This project implements an end-to-end machine learning pipeline to predict
short-term aircraft trajectories using real ADS-B state vector data from the
OpenSky Network. An LSTM neural network is trained to learn temporal motion
patterns and predict the next position of an aircraft.

---

## 🚀 Project Overview

- **Domain:** Aeronautics / Aviation AI  
- **Task:** Time-series trajectory prediction  
- **Aircraft Type:** Commercial aircraft (ADS-B data)  
- **Model:** LSTM (Long Short-Term Memory)  
- **Framework:** TensorFlow / Keras  

The objective is to demonstrate how real-world aviation data can be cleaned,
processed, and used to train a deep learning model for trajectory prediction.

---

## 📊 Data Source

- **Dataset:** OpenSky Network – ADS-B State Vector Data  
- **Sampling Rate:** 10 seconds  
- **Features Used:**
  - Latitude
  - Longitude
  - Velocity
  - Heading
  - Barometric altitude

Only airborne aircraft were considered, and a single aircraft trajectory was
extracted for modeling.

---

## 🛠️ Methodology

1. **Data Acquisition**
   - Load real ADS-B state vector data from OpenSky

2. **Data Cleaning & Preprocessing**
   - Remove ground states
   - Handle missing values
   - Convert timestamps
   - Sort data by aircraft and time

3. **Time-Series Preparation**
   - Extract a single aircraft trajectory
   - Normalize features
   - Create sliding windows for LSTM input/output

4. **Modeling**
   - LSTM-based neural network
   - Mean Squared Error (MSE) loss
   - Adam optimizer

5. **Evaluation**
   - Training vs validation loss analysis
   - Predicted vs actual trajectory visualization

---

## 📈 Results

The trained LSTM model successfully learns short-term aircraft motion patterns.
Predicted trajectories closely follow the real aircraft path, demonstrating
the model’s ability to capture temporal dependencies in ADS-B data.

Example result:

- **Training & validation loss convergence**
- **Predicted vs actual trajectory (latitude vs longitude)**

---

## 🔮 Future Improvements

- Multi-step trajectory prediction
- Training on multiple aircraft
- Incorporating weather or wind data
- Trying sequence-to-sequence or Transformer models

---

## 📂 Repository Structure

