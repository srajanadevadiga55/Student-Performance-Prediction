# Student Performance Prediction

## Project Overview
This project uses Machine Learning to predict students' final mathematics grades based on student-related information. Three regression models are trained and compared to evaluate their prediction performance.

## Objective
The main objective is to predict a student's final mathematics grade (G3) using available student information.

## Dataset
The project uses the Student Performance dataset containing student-related information.

- **Target variable:** G3 (final mathematics grade)
- **Input features:** Student-related numerical and categorical information
- **Excluded features:** G1 and G2 (previous grades), to avoid using previous grades as inputs.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## Project Workflow
1. Load and explore the dataset.
2. Check the dataset structure and missing values.
3. Separate input features and target variable.
4. Split the data into training and testing sets (80% training and 20% testing).
5. Preprocess numerical and categorical features.
6. Train three regression models:
   - Baseline Regression
   - Linear Regression
   - Random Forest Regression
7. Evaluate the models using MAE, RMSE, and R² score.
8. Perform five-fold cross-validation.
9. Visualize model performance.
10. Analyze feature importance.
11. Generate a sample prediction.
12. Save the trained model and evaluation results.

## Model Evaluation
The models are compared using:
- **MAE:** Mean Absolute Error
- **RMSE:** Root Mean Squared Error
- **R² Score:** Coefficient of Determination

Lower MAE and RMSE generally indicate better predictions. A higher R² score generally indicates that the model explains more variation in the target.

See `model_evaluation_results.csv` for the actual evaluation results.

## Project Files
- `Student_Performance_Prediction.ipynb` — notebook containing code, analysis, charts, and predictions.
- `student_performance_model.pkl` — saved Random Forest model and preprocessing pipeline.
- `model_evaluation_results.csv` — model evaluation results.
- `Student_Performance_Project.zip` — ZIP archive of supporting project files.

## Limitations
- Predictions are estimates and may differ from actual grades.
- The dataset may not represent all students or schools.
- Model performance depends on the quality and relevance of the dataset.
- Feature importance does not prove that a feature causes a particular grade.

## Future Improvements
- Test additional machine learning algorithms.
- Evaluate the model on a larger and more diverse dataset.
- Develop a simple web application for predictions.

## Disclaimer
This project is created for educational purposes as part of a machine learning internship task. Predictions should not be used as the sole basis for important decisions about students.
