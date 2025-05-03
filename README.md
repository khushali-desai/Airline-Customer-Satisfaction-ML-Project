# ✈️ Airline Customer Satisfaction Prediction

This project focuses on predicting airline customer satisfaction using a **Decision Tree Classifier**. The dataset includes features such as gender, customer type, age, class, type of travel, flight distance, and various service ratings.

The goal is to classify whether a customer is **satisfied** or **not satisfied** based on these attributes. This project demonstrates end-to-end data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and evaluation using a Decision Tree.

---

## 📁 Dataset Overview

The dataset includes the following key features:

- **Demographic Information**: Gender, Age, Customer Type
- **Flight Information**: Class, Type of Travel, Flight Distance, Departure/Arrival Delays
- **Service Ratings**: Ratings for Inflight Service, Cleanliness, Food and Drink, etc.
- **Target Variable**: `satisfaction` (encoded as 1 for Satisfied, 0 for Neutral or Dissatisfied)

---

## 🔧 Steps Performed

### 1. Data Preprocessing

- Removed unnecessary columns (like `Unnamed: 0`)
- Replaced spaces in column names with underscores for consistency
- Handled missing values by dropping rows with `NaN`
- Encoded the target variable (`satisfaction`) using binary mapping
- Applied **Label Encoding** for categorical features

### 2. Exploratory Data Analysis (EDA)

- Used **Seaborn** and **Matplotlib** for visualizing:
  - Distribution of satisfaction across classes and types of travel
  - Correlation heatmap between features
  - Count plots for categorical features
- Identified key patterns like higher satisfaction in Business Class and among Loyal Customers

### 3. Feature Scaling

- Used **StandardScaler** to normalize numerical features such as `Age`, `Flight Distance`, and delays.

### 4. Model Building

- Split data into training and testing sets (80/20 split)
- Trained a **Decision Tree Classifier** using scikit-learn

### 5. Model Evaluation

The performance of the model was evaluated using multiple metrics:

- **Accuracy Score**: `0.946`
- **Precision Score**: `0.95`
- **Recall Score**: `0.94`
- **F1 Score**: `0.94`
- **Confusion Matrix** and **Classification Report** were also generated for a detailed breakdown.

---

## 📌 Key Findings

- **Loyal Customers** and **Business Class** travelers were more likely to be satisfied.
- Decision Tree performed well with a high accuracy and balanced precision/recall.
- Features like `Inflight_wifi_service`, `Online_boarding`, and `Seat_comfort` had noticeable influence on satisfaction.

---

## 🛠️ Tools & Libraries Used

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (DecisionTreeClassifier, metrics, preprocessing)

---

## 📊 Conclusion

This project successfully demonstrates how a **Decision Tree model** can be used to predict customer satisfaction with high accuracy using a clean and interpretable set of features. The workflow included complete preprocessing, meaningful EDA, and a well-evaluated model.

---

## 📌 Author

This project was solely developed and implemented by the author using personal code and analysis.

