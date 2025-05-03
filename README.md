# ✈️ Airline Customer Satisfaction ML Project

This Machine Learning project predicts airline customer satisfaction using a **Decision Tree Classifier**. The project was implemented in **Jupyter Notebook** and follows a complete machine learning pipeline from preprocessing to model evaluation.

---

## 📁 Dataset Overview

The dataset includes the following features:

- **Demographics**: Gender, Age, Customer Type
- **Flight Details**: Class, Type of Travel, Flight Distance, Departure and Arrival Delays
- **Service Ratings**: Seat comfort, Cleanliness, Food and Drink, etc.
- **Target Variable**: `satisfaction` (1 = Satisfied, 0 = Not Satisfied)

---

## 🔧 Project Workflow

### 1. Data Preprocessing

- Removed the `Unnamed: 0` column
- Dropped rows with missing values
- Replaced spaces in column names with underscores
- Converted the `satisfaction` column into binary format (1 and 0)
- Applied **Label Encoding** to categorical variables

### 2. Exploratory Data Analysis (EDA)

- Visualized customer satisfaction distribution
- Analyzed relationships between satisfaction and features like travel class and customer type
- Created a correlation heatmap using seaborn

### 3. Feature Scaling

- Applied `StandardScaler` to numerical features for model training

### 4. Model Building

- Used **DecisionTreeClassifier** from scikit-learn
- Split the data into training and testing sets using an 80/20 ratio

### 5. Model Evaluation

The Decision Tree model performance:

- **Accuracy Score**: `0.9154694286668894`
- **Recall Score**: `0.8987730061349694`
- **F1 Score**: `0.9025798998844821`
- **Precision Score**: `0.9064191802010828`

A classification report and confusion matrix were also generated.

---

## 🛠️ Tools Used

- Python (Jupyter Notebook)
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn (DecisionTreeClassifier, metrics, preprocessing)

---

## 🧑‍💻 Author

This project was fully implemented by the author using Jupyter Notebook. All analysis, visualization, and model training were done from scratch using personal code.
