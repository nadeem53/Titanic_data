# Titanic_data

## Titanic Dataset Machine Learning Project

This repository contains the code and data for a machine-learning project to predict the survival rates of passengers on the Titanic. The project uses the Titanic dataset, which contains information on over 2,200 passengers, including their age, sex, class, and ticket fare.

# To run the project:

Clone the repository to your local machine.
Install the required Python libraries:
-numpy

-pandas

-scikit-learn

-seaborn

-matplotlib

Run the following command to train and evaluate the machine-learning model:
python titanic_ml.py
The output of the script will be the accuracy of the model on the test set.

To use the model to predict the survival rate of a new passenger:

Create a new Python file and import the following libraries:

numpy
pandas
pickle
Load the trained model:

model = pickle.load(open('model.pkl', 'rb'))
Create a new data frame with the features of the new passenger:

new_passenger = pandas.DataFrame({'Age': [25], 'Sex': ['male'], 'Pclass': [1], 'Fare': [100]})
Predict the survival rate of the new passenger:

survival_rate = model.predict_proba(new_passenger)[0][1]
Print the survival rate:

print(survival_rate)
This project is still under development, but it has already achieved an accuracy of over 80% on the test set. I am working on improving the accuracy of the model and adding new features, such as cabin class and family size.

Please feel free to contribute to the project or use it for your own machine-learning projects.
