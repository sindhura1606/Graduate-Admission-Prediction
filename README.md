# Graduate Admission Prediction
 
Introduction:
Every university has certain aspects that determines student acceptance into the university
The objective is to explore the dataset and features provided to determine most significant features that contribute the most to student chance of a admission
Finally, define a model to predict probability of the admission

Dataset:
The dataset we choose is Graduate Admissions Dataset from Kaggle
It consists of 500 records and 8 	features
GRE Score
TOEFL Score
University Ratings
Statement of Purpose(SOP) Score
Letter of Recommendation(LOR) Score
CGPA
Whether the Student Has Done Any Research
Chance of Admission (What We're Trying to Predict)


Data Preparation and Exploration:
Almost many datasets will have a lot of anomalies like missing values and outliers
Fortunately, there are no missing values in our dataset
Serial no is just an index for students which can be taken out
However, LOR Feature has an outlier
observe few values that fall under  the range
    1.0, where as rest of the values are between
    3.0 to 4.0
Criteria to find outliers is using IQR(Q3-Q1)
	Q3+1.5 x (IQR) (any value > than this is suspected outlier)
	Q1-1.5 x (IQR)  (any value > than this is suspected outlier)

Data Preparation and Exploration contd..:
A heat map is used to see the correlation of all the features compared to Chance to Admit:
The top three features that affect the Chance to Admit are:
CGPA
GRE Score
TOEFL Score

Business use case:
1)Through this project the students can calculate his chance of admit and their requirements for their admission
2)From our first hypothesis we are going to know if all the predictors are important to determine the grad admission. CGPA, TOEFL, GRE score has the highest percentage to determine the chance of admit 
3)From the second use case we are considering how much does GRE and TOEFL influence the chance of admittance
4)From the third use case we are considering how much does Research and CGPA influence the Chance of Admittance.
5)From the fourth use case we are considering how much does SOP and LOR matter influence the Chance of Admittance
6)From the fifth use case we are considering how much does University Rating and CGPA influence the Chance of Admittance.


