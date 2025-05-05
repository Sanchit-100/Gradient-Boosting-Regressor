# 🌲 Gradient Boosting Regressor from Scratch

This repository implements **Gradient Boosting Regression** using **Decision Stumps** as weak learners, built from scratch using NumPy. The model is evaluated on a synthetic dataset under both **Mean Squared Error (MSE)** and **Mean Absolute Error (MAE)** loss functions.

---

## 📊 Dataset Description

- **Input (x)**: 100 points sampled from a uniform distribution [0,1]
- **Target (y)**: Generated using the function:
                    y = sin(2πx)+cos(2πx)+ gaussian noise

- **Train-Test Split**: 80% training, 20% testing
- **Noise**: Gaussian noise with mean 0 and standard deviation 0.01

---

## 🧠 Model Features

- **Base Learner**: Decision Stump Regressor
- **Boosting Method**: Gradient Boosting
- **Learning Rate**: 0.01
- **Iterations**: Configurable (default: 2000)
- **Loss Functions Supported**:
  - MSE (Mean Squared Error)
  - MAE (Mean Absolute Error)
- **Gradient Calculation**:
  - For MSE: - (y_true - y_pred)
  - For MAE: - sign (y_true - y_pred)
- **Stump Splitting Strategy**: 20 equally spaced thresholds in [0, 1]

---

## 🧪 Performance

- ✅ **Test MSE (Squared Loss)**: `0.01600`
- ✅ **Test MAE (Absolute Loss)**: `0.09360`

---

## 📈 Visualizations

### 📌 Dataset Visualization
> Shows scatter plot of training and testing data.

**[Insert Dataset Plot Here]**

---

### 🔁 Training Loss over Iterations

- **MSE Loss**:

![image](https://github.com/user-attachments/assets/aeef4f4c-29bf-46d6-807e-5d1315de6541)


- **MAE Loss**:

![image](https://github.com/user-attachments/assets/decb8cd4-b41d-4210-9b33-ffc2f8024861)


---

### 📊 Predictions vs Ground Truth

- **Test Set Predictions (MSE Loss)**
![image](https://github.com/user-attachments/assets/98721e97-a7c0-4093-9706-0b5e365e3881)


- **Train Set Predictions (MSE Loss)**
- ![image](https://github.com/user-attachments/assets/8f5bb0da-701a-4c93-b1c4-7c32b8cb9324)




---

- **Test Set Predictions (MAE Loss)**

![image](https://github.com/user-attachments/assets/844ce111-1154-4f6c-bff0-06e56db54265)


- **Train Set Predictions (MAE Loss)**

![image](https://github.com/user-attachments/assets/b2df1091-9b13-4e63-a6e1-bbc1368cbcb3)


