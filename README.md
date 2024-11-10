### **Stroke Prediction Model using Machine Learning**

This project aims to predict whether a patient is at risk of having a stroke based on various medical attributes, including lifestyle factors and health conditions. The dataset used includes information about demographics, medical history, and lifestyle choices to predict the likelihood of a stroke. 

### **Objective:**
The goal of this project is to leverage machine learning models to accurately predict the likelihood of a stroke, helping medical professionals identify high-risk individuals and make informed decisions for early intervention.

### **Key Features:**
- **Data Attributes:**  
  - **Gender:** Male, Female, or Other  
  - **Age:** The age of the patient  
  - **Hypertension:** 1 if the patient has hypertension, 0 otherwise  
  - **Heart Disease:** 1 if the patient has a heart condition, 0 otherwise  
  - **Ever Married:** Whether the patient has ever been married  
  - **Work Type:** Employment status (Govt job, Private, Self-employed, Never worked)  
  - **Residence Type:** Urban or Rural  
  - **Average Glucose Level:** Blood sugar levels of the patient  
  - **BMI:** Body Mass Index  
  - **Smoking Status:** Whether the patient is a smoker, ex-smoker, or non-smoker  

- **Outcome:**  
  The target variable, `stroke`, is a binary classification (1 if the patient has had a stroke, 0 if not).

### **Models Used:**
The project utilizes several machine learning models to predict stroke occurrence:

1. **Random Forest Classifier**  
   - The Random Forest model is trained on various health and lifestyle factors to predict whether a person has had a stroke. The model achieves an impressive accuracy of **94.28%** on the test set.
   
2. **Decision Tree Classifier**  
   - A Decision Tree model was used to identify the most important features influencing stroke prediction. The `avg_glucose_level` was identified as one of the most significant factors.

3. **Feature Importance Visualization:**  
   - Using the Decision Tree model, the feature importance values were calculated and visualized, showing how each factor contributes to the prediction. The top features influencing stroke risk include **average glucose level**, **BMI**, and **age**.

### **Data Preprocessing:**
- **Standardization:**  
  Data was standardized using the `StandardScaler` to ensure that all features are on a similar scale, improving model performance.
  
- **Train-Test Split:**  
  The dataset was split into training (80%) and testing (20%) sets to evaluate model performance.

### **Prediction Process:**
- The model allows user input for key attributes, including gender, age, medical history (hypertension, heart disease), marital status, lifestyle factors (work type, smoking status), and more. Based on these inputs, the model predicts whether the individual is at risk of having a stroke.

### **Performance Metrics:**
- **Random Forest Classifier Accuracy:** 94.28%  
- **Decision Tree Classifier Accuracy:** 91.67%  
- **Confusion Matrix & Classification Report:**  
  - The confusion matrix and classification report evaluate model performance in terms of precision, recall, and F1-score.

### **Risk Factor Analysis:**
- The project also explores how various factors such as **age**, **glucose level**, and **BMI** contribute to the likelihood of a stroke, with visualizations showing how different demographics and health conditions affect stroke risk.

### **Visualization:**
- **Feature Importance Plot:** Displays the relative importance of features used in stroke prediction.
- **Risk Factor Visualizations:** Bar charts comparing stroke rates across different demographic and health-related factors.

### **Future Enhancements:**
- The model can be further enhanced by including additional health conditions or integrating real-time data.
- Other advanced machine learning models like XGBoost or neural networks can be explored for potentially higher accuracy.
  
### **Conclusion:**
This project demonstrates the power of machine learning in healthcare, specifically in stroke prediction. By combining various health attributes, the model can assist in identifying individuals at risk and potentially save lives by enabling timely medical intervention.

---

