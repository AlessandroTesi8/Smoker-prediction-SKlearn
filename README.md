# Binary Prediction of Smoker Status using Bio-Signals

This Jupiter notebook provides a comprehensive guide for predicting an individual's smoking status using bio-signals through various machine learning models. The project encompasses a thorough analysis of the dataset, extensive feature engineering, model selection and optimization, and the final evaluation of the best model. Below is the structure of the notebook:

## Index

### Preparing Environment and Data
In this section, we set up our working environment and prepare our dataset for analysis.
- **Importing Libraries**: Load all necessary Python libraries for data manipulation, analysis, and modeling.
- **Loading the Dataset**: Import the dataset that contains bio-signals and smoking status.
- **Dirtying the Dataset**: Intentionally introduce some 'dirt' into the dataset for demonstrating cleaning techniques (optional step for educational purposes).

### Data Analysis
This part focuses on understanding and cleaning the dataset.
- **Analysis of the Missing Values with Missingno and Dropping Useless Rows**: Use Missingno library to visualize missing values, and remove rows that do not contribute to the prediction.
- **Train & Test Split**: Split the dataset into training and testing sets to ensure the model can be validated independently.
- **Analysis of Feature Values, Distributions, and Correlations**: Examine how the features are distributed and their correlations with each other.

### Feature Engineering & Preprocessor Pipeline Creation
Enhance the dataset with new features and prepare it for modeling.
- **Build Custom Pipelines to Create New Features**: Including BMI (Body Mass Index), Eyesight, Pulse Pressure, Blood Pressure, and AST/ALT ratio.
- **Create Pipelines for Imputing & Scaling**: Handle missing values and scale features to prepare for modeling.
- **Compose the Final Preprocessor**: Combine all preprocessing steps into a single pipeline for convenience.

### Model Selection
Evaluate various classifiers to select the most promising ones.
- **Evaluation of the Performance of Each Classifier via Cross-Validation**: Test multiple models, such as Dummy, Logistic Regression, KNN, SVM, Decision Tree, Random Forest, GBM, AdaBoost, and XGBoost, to gauge their initial performance.
- **Refinement of the Best Models via Random Search**: Focus on PCA, LDA, Random Forest, GBM, and SVM for hyperparameter tuning using random search.

### Best Model Hypertune
Fine-tune the best model to optimize its performance.
- **Fine Tune of the Best Classifier via Successive Halving**: Use advanced techniques to narrow down the best settings for the model.
- **Build Train-Validation Accuracy and Reduce Overfitting**: Aim to improve the model's accuracy on unseen data while preventing overfitting.
- **Build ROC Curve**: Evaluate the model's performance in classifying the positive class in the dataset.
- **Tune the Threshold**: Adjust the decision threshold to balance the trade-off between sensitivity and specificity.

### Final Model Evaluation
Conduct a comprehensive evaluation of the final model.
- This section focuses on assessing the tuned model's performance on the test set, including its accuracy, precision, recall, F1 score, and other relevant metrics to ensure its reliability in predicting smoker status based on bio-signals.

This notebook is structured to guide you through every step of the machine learning pipeline, from data preparation to the final evaluation of the model. Whether you are a beginner or an experienced data scientist, this project offers valuable insights into the process of developing a predictive model using real-world data.
