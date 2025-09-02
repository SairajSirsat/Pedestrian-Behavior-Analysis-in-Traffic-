# 🚶 Pedestrian Behavior Analysis in Traffic Using Machine Learning

This project applies **Machine Learning** to analyze and model pedestrian behavior in traffic. It uses regression, classification, and clustering techniques to understand pedestrian movement, detect behavioral patterns, and predict pedestrian actions. Such insights are valuable for **urban planning, road safety, and autonomous vehicle navigation**.

---

## 📌 Problem Statement
Pedestrian behavior in traffic is complex and influenced by multiple factors such as movement speed, direction, density, and crossing patterns.  
The main objectives of this project are:
1. **Regression** → Predict pedestrian movement variables like position, speed, and acceleration.  
2. **Classification** → Identify pedestrian behavior types (e.g., safe vs. risky).  
3. **Clustering** → Detect pedestrian zones and group similar movement patterns.  

---

## 📂 Dataset
- The dataset (`tracks.csv`) contains pedestrian tracking data with attributes such as **position (x, y), time, body orientation, and movement sequences**.  
- Preprocessing included:  
  - Handling missing values  
  - Normalization of x, y coordinates  
  - Outlier removal using Z-scores  
  - Feature engineering (speed, acceleration)  

*(Dataset not included due to size/privacy; users can add their own pedestrian datasets.)*

---

## ⚙️ Methodology

### 🔧 Data Preprocessing
- Cleaned list-like columns stored as strings  
- Replaced missing values in orientation features  
- Normalized **x, y coordinates**  
- Removed duplicates and outliers  

### 📊 Exploratory Data Analysis (EDA)
- Histograms & distributions of pedestrian features  
- Scatter plots of pedestrian movement patterns  
- Boxplots for outlier detection  

### 🏗️ Feature Engineering
- Computed **Speed** (distance/time)  
- Computed **Acceleration** (change in speed/time)  

### 📈 Models Applied
#### Regression
- Linear Regression  
- Random Forest Regressor  
- XGBoost Regressor  
- Support Vector Regression (SVR)  

#### Classification
- Logistic Regression  
- Random Forest Classifier  
- Naive Bayes  
- Support Vector Classifier (SVC)  

#### Clustering
- **K-Means** → Grouping pedestrians by similarity  
- **DBSCAN** → Detecting clusters + outliers  

### 🧪 Evaluation Metrics
- **Regression**: MAE, MSE, RMSE, R²  
- **Classification**: Accuracy, Precision, Recall, F1-score, Confusion Matrix  
- **Clustering**: Cluster visualization and interpretation  

---

## 📊 Results
- **Regression**: Captured pedestrian movement trends (speed, acceleration).  
- **Classification**: Random Forest achieved high accuracy in behavior categorization.  
- **Clustering**: K-Means and DBSCAN revealed meaningful pedestrian groupings.  

*(Update this section with your actual accuracy, F1-score, RMSE, etc.)*

---

## 🚀 Future Work
- Apply **deep learning models** (LSTM, CNNs) for sequential and image-based pedestrian data.  
- Deploy as a **real-time pedestrian behavior monitoring system**.  
- Extend to **multi-modal data** (traffic cameras + sensor data).  

---

## 🛠️ Installation & Usage
Clone this repository:
```bash
git clone https://github.com/your-username/pedestrian-behavior-analysis.git
cd pedestrian-behavior-analysis
