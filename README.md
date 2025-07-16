# BUILD-AND-VISUALIZE-A-DECISION-TREE-MODEL
COMPANY: CODTECH IT SOLUTIONS
NAME: ABHIJEET KUMAR
INTERN ID: CTO4DG2125
DOMAIN: MACHINE LEARNING
DURATION: 4 WEEKS
MENTOR: NEELA SANTOSH
DESCRIPTION : 
In this task our goal is to predict whether a person has diabetes or not based on medical measurements, such as glucose level, BMI, insulin level, and more. I use a well-known dataset called the Pima Indians Diabetes dataset and apply a Decision Tree algorithm from the scikit-learn library to build a predictive model.

Step 1: Import all the Library of Python
Step 2: Load and Understanding the Dataset
The Diabetes dataset contains 768 records with 8 features (independent variables) and 1 target variable (Outcome). The target variable is either:
1 → the person is diabetic, 0 → the person is not diabetic.
The features include:
Pregnancies, Glucose, BloodPressure, SkinThickness, Insulin, BMI, DiabetesPedigreeFunction, Age

Step 3: Loading and Preparing the Data
By importing Python libraries like pandas, numpy, and matplotlib for data handling and visualization.
Then, load the dataset using pandas.read_csv() and check for any missing values or irregularities.
After ensuring the dataset is clean, we split the data into:
X: the input features (all columns except Outcome)
y: the target column (Outcome)

Step 4: Train and Test Split
To evaluate the model fairly, I split the dataset into two parts:
Training set (80%): Used to train the decision tree.
Test set (20%): Used to evaluate model performance.
This is done using train_test_split() from sklearn.model_selection.

Step 6: Training the Decision Tree Model
Then, I use the DecisionTreeClassifier from sklearn.tree. 
The tree learns rules from the training data. We can customize it using parameters like:
criterion='entropy': to use information gain.
max_depth=4: to avoid making the tree too complex and overfitting the data.

Step 7: Visualizing the Decision Tree
Using plot_tree() function, I create a visual representation of the tree.
This visualization shows how the model splits data at each level, based on conditions like "Is Glucose > 127?". 
Leaf nodes show the predicted class (diabetic or not), which makes it easy to understand how the model makes decisions.

 Step 8:  Making Predictions and Evaluating the Model
After the model is trained, I use it to predict values for the test data (y_pred). then evaluate the model using:
Accuracy Score: How many predictions are correct.
Classification Report: Includes precision, recall, and F1-score.
Confusion Matrix: A table that shows actual vs predicted classes, helping identify misclassifications.

Step 9: Plotting the Confusion Matrix
A heatmap using seaborn.heatmap() helps visually show how well the model performed — 
how many cases were correctly or incorrectly classified as diabetic or not diabetic.
#OUTPUT:-
<img width="1716" height="721" alt="Image" src="https://github.com/user-attachments/assets/a5dac6a2-e757-4918-a1d4-4b259e19155a" />
<img width="1192" height="751" alt="Image" src="https://github.com/user-attachments/assets/a7cbfb48-2181-482f-b65e-925722b43833" />
