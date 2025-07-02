
# 🍽️ Dynamic Diet Recommendations with Real-Time Data for Personalized Nutrition

## 📌 Overview

This project presents a **Dynamic Diet Recommendation System** that leverages **real-time data** and **machine learning** to generate personalized diet plans. Unlike traditional static meal plans, this system adapts to the user's changing health conditions, nutritional needs, and activity levels.

Built with a **Multi-Layer Perceptron (MLP)** using **Keras**, the system classifies food items into goals such as **Weight Gain**, **Muscle Gain**, and **General Food**, providing intelligent and flexible dietary suggestions.

---

## 🧠 Features

- Personalized diet recommendations using user-specific health data
- Real-time adaptability using continuously updated inputs
- Multi-class classification of food based on nutritional content
- Performance visualization (accuracy, loss, confusion matrix)
- Comparative model performance analysis (CNN, RNN, LSTM, SVM)

---

## 🧪 Dataset

The dataset includes **4,684 food items** categorized into:
- Weight Gain
- Muscle Gain
- General Food

Each food item contains:
- **Macronutrients**: Energy (kcal), Protein (g), Fat (g), Carbs (g), Fiber (g), Sugar (g)
- **Micronutrients**: Vitamin A, Calcium, Iron, etc. (% of USRDA)

It also includes:
- Food group classification (e.g., Legumes, Baked Products, Finfish)
- Unique food IDs and names for identification

---

## 🔍 Methodology

### Preprocessing
- Handling missing values
- Feature engineering (e.g., protein-to-fat ratio)
- One-hot encoding of target classes

### Model Architecture
- Input Layer: 64 neurons
- Hidden Layer: 32 neurons (ReLU activation)
- Output Layer: 3 neurons (SoftMax for multiclass)

### Training
- Optimizer: Adam
- Epochs: 50
- Batch size: 32

---

## 📊 Results

### Classification Report

| Category      | Precision | Recall | F1-Score |
|---------------|-----------|--------|----------|
| Weight Gain   | 0.85      | 0.80   | 0.82     |
| Muscle Gain   | 0.90      | 0.92   | 0.91     |
| General Food  | 0.78      | 0.75   | 0.76     |
| **Average**   | **0.84**  | **0.82** | **0.83** |

### Performance Comparison

| Model         | Accuracy | F1-Score |
|---------------|----------|----------|
| Neural Network| 84.0%    | 83.0%    |
| CNN           | 88.5%    | 88.0%    |
| LSTM          | 86.0%    | 85.7%    |
| RNN           | 82.5%    | 81.7%    |
| SVM           | 80.0%    | 78.8%    |

---

## 💡 Key Insights

- CNN outperforms traditional models in accuracy and generalization.
- The model performs best for **Muscle Gain** classification.
- Misclassifications between “General Food” and “Weight Gain” occur due to overlapping nutritional content.

---

## 🔭 Future Scope

- Integration with **IoMT** (Internet of Medical Things) and wearable devices
- Use of **advanced biomarkers** (HRV, lipid profiles) for precise monitoring
- Expansion to handle **chronic disease-specific diets**
- Deployment as a **mobile or web-based app**
- Use of **transfer learning, CNN/RNN hybrids**, and **real-time feedback loops**

---



