#  Comparison Report Between Logistic Regression & Neural Networks

##  Overview
This project focuses on **human activity recognition** using motion sensor data. Two machine learning models — **Logistic Regression** and a **Neural Network (MLP Classifier)** — are implemented and compared in terms of their ability to classify activities like *Rub Hands* and *Open Door* based on accelerometer and gyroscope readings.

---

##  Objective
To evaluate the performance of classical and neural approaches for activity recognition using extracted features from motion sensor data.

---

##  Dataset
The dataset consists of **accelerometer** and **gyroscope** readings collected through motion sensors.  
Each data sample represents a specific activity:

- **Activity Classes:** Rub Hands, Open Door  
- **Sensors Used:** MSAccelerometer & MSGyroscope  
- **Data Split:** Training and testing sets are stored in `.npy` format.

---

##  Feature Extraction
From each (X, Y, Z) axis reading, the following statistical features were extracted:
- Mean  
- Standard Deviation  
- Minimum  
- Maximum  

Each sensor contributes 12 features →  
For both sensors combined → **24 features per sample**.

---

##  Models Implemented
### 1. Logistic Regression
- Baseline linear model  
- `max_iter = 1000`  

### 2. Neural Network (MLPClassifier)
- Hidden Layer: 2 layers with 64 neurons and 25 neurons  
- `max_iter = 500`, `random_state = 42`

---

##  Results Summary
| Model | Accuracy | F1 Score |
|--------|-----------|----------|
| Logistic Regression | **0.9444** | **0.9443** |
| Neural Network (MLP) | **0.9667** | **0.9666** |

Both models performed well, with **MLP Classifier** expected to slightly outperform Logistic Regression due to its ability to capture non-linear relationships in sensor data.

---

##  Visualizations
Confusion matrices for both models are plotted side by side for better comparison:  
- Left: Logistic Regression  
- Right: MLP Classifier  

---

##  Tech Stack
- Python  
- NumPy  
- scikit-learn  
- Matplotlib  
- Seaborn  

---

##  How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/AneebaWaseem/LogisticRegression-and-NeuralNetworks
   cd LogisticRegression-and-NeuralNetworks
   ```

2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook ComparisonReport.ipynb
   ```

3. Run all cells sequentially to reproduce results and visualizations.

---

##  Conclusion
This study highlights that:
- **Logistic Regression** serves as a strong baseline for sensor-based activity recognition.
- **Neural Networks (MLP)** provide better adaptability to complex, non-linear feature relationships.
- Feature engineering (mean, std, min, max) plays a crucial role in model performance.

---

**Aneeba Waseem**  
📅 *2025*  
🎓 Project: *Comparison Report between Logistic Regression & Neural Networks*  
