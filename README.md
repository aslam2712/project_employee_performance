# project_employee_performance

Reqiuerment 1 : 
			Department wise performances:


File saved as project_employee_performance\src\data processing\data_processing_department_wise_analysis

- Imported pandas and numpy.
- Loaded data
- Arranged data by Using Group by and Gruoped data on Basis on EmpDepartment.
data_dep = data_1.groupby(data_1['EmpDepartment'])

-calculated  mean of grouped data.
- this gives performance Rating based on EmpDepartment

- Also plotted graph using Tableau to visualize data . scrren shoot of Tableau is attached in 
project_employee_performance\src\visualization

				Final Result :
Development : 3.05
Data Science : 3.05
Human Resource : 2.92



				Requirement 2 : 
		Top 3 Important Factors effecting employee performance
-File saved as Most_effective_parameter in location
project_employee_performance\src\data processing
-Loaded Numpy , pandas , rcParams, ststsmodel.formula.api
-Generated summary considering all Parameters :
- observed p-value of all the features and removed feature with max p- value
-continued to remove parameters untill all features were left with p-value less then .05
        
		Final result: Most effective parameters are:
1.EmpLastSalaryHikePercent (has p value 0.000 and std err is very small) 
2.ExperienceYearsInCurrentRole 
3.YearsSinceLastPromotion 



				Requirement 3
A trained model which can predict the employee performance based on factors as inputs. 
This will be used to hire employees
 
-Imported Numpy, panads , seed, randrange, sqrt
- Loaded data.
-Imported train_test_split
- Loaded all features in X and performance (last column) in y.
- splitted data in training data and test data using Train_test_split
- used RandomForestClassifier to Train Data.
-Fitted X_train and y_Train to train model.
- calculated predictions with reference on X_test
- calculated error , by substracting pridiction from actual y_test.
- calculated mean absolute percentage error.
- calculated accuracy.
Its out to be 84.07%


			Requirement 4:
Recommendations to improve the employee performance based on insights from analysis.

- Based on all out put we can suggest following Point:

- people on development have best performance .
- Salary hike is most important feature in performance that should be given more waightage.
- Employee shall be hired on basis for specific Role with relevant experince in that role .
- promotions shall be given on regualr Interval that keeps Employee motivated.
- we can use RandomForestClassifier model and put all features as input while hiring new employess and predicted performance shall be as accuarte as 84%.
