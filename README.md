# 🏭 Machine Failure Prediction using Decision Trees

## 📌 Problem Statement

**AutoMobi Engineering Pvt. Ltd.** is an auto component manufacturing company that operates several critical machines. Predictive maintenance is crucial for the company to reduce downtime, save costs, and ensure production efficiency. This project uses machine learning techniques to build a model that predicts machine failure before it occurs.

## 🎯 Objective

- Predict the probability of machine failure using historical sensor and operational data
- Use a Decision Tree Classifier to identify key features influencing failures
- Help the organization move from reactive to proactive maintenance

## 📊 Dataset

- **File**: `machine_failure_data.csv`
- **Target Variable**: `machine_failure` (binary: 0 = No Failure, 1 = Failure)
- **Features Include**:
  - `Air temperature`, `Process temperature`
  - `Rotational speed`, `Torque`, `Tool wear`
  - Categorical variables like `Type`, and individual failure types (e.g., `TWF`, `HDF`, `OSF`, etc.)

## 📁 Repository Structure

```
├── MLS2_DecisionTree_MachineFailurePrediction.ipynb   # Main notebook
├── machine_failure_data.csv                           # Dataset file
├── README.md                                          # Project documentation
```

## 🧪 Project Workflow

1. **Data Exploration & Preprocessing**
   - Checked for missing values and balanced class distribution
   - Converted categorical features into numerical form
   - Combined failure indicators into a single binary `machine_failure` label

2. **Exploratory Data Analysis**
   - Analyzed feature distributions and correlations
   - Visualized machine failure trends across machine types and operating conditions

3. **Model Building**
   - Used `DecisionTreeClassifier` from `sklearn`
   - Performed train/test split
   - Tuned hyperparameters (e.g., `max_depth`, `min_samples_split`)

4. **Model Evaluation**
   - Confusion matrix
   - Accuracy, Precision, Recall, and F1 Score
   - Visualized the decision tree for interpretability

## 🏆 Results

- **Accuracy Achieved**: ~91%
- **Important Predictors**:
  - `Tool wear` and `Rotational speed` showed strong influence on machine failure
- **Business Value**:
  - Early identification of failure risks
  - Improved scheduling of maintenance activities

## 🔍 Takeaways

- Decision Trees offer great interpretability, making them suitable for industrial use cases
- Key sensor indicators such as torque and temperature can act as early warnings
- Preventive maintenance powered by ML can reduce operational cost and avoid unplanned downtime

## 🚀 Future Enhancements

- Try ensemble models like Random Forest and XGBoost for improved performance
- Integrate with IoT platforms for real-time monitoring and prediction
- Explore time-series modeling for more dynamic machine health forecasting

## 👨‍💻 Author

**Suhaib Khalid**  
ML Practitioner
