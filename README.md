# Neural Network Challenge
Module 18 

**Background**

You work at a company that specializes in student loan refinancing. If the company can predict whether a borrower will repay their loan, it can provide a more accurate interest rate for the borrower. Your team has asked you to create a model to predict student loan repayment.
The business team has given you a CSV file that contains information about previous student loan recipients. With your knowledge of machine learning and neural networks, you decide to use the features in the provided dataset to create a model that will predict the likelihood that an applicant will repay their student loans. The CSV file contains information about these students, such as their credit ranking.

**Instructions**
Open the starter file in Google Colab and complete the following steps, which are divided into four parts:
1. Prepare the data for use on a neural network model.
2. Compile and evaluate a model using a neural network.
3. Predict loan repayment success by using your neural network model.
4. Discuss creating a recommendation system for student loans.

**Part 1: Prepare the data for use on a neural network model**

Using your knowledge of Pandas and scikit-learn’s StandardScaler(), preprocess the dataset so that you can use it to compile and evaluate the neural network model later.
Open the starter code file and complete the following data preparation steps:
1. Read the data from https://static.bc-edx.com/ai/ail-v-1-0/m18/lms/datasets/student-loans.csv Links to an external site. into a Pandas DataFrame. Review the DataFrame, looking for columns that could eventually define your features and target variables.
2. Create the features (X) and target (y) datasets. The target dataset should be defined by the “credit_ranking” column. The remaining columns should define the features dataset.
3. Split the features and target sets into training and testing datasets.
4. Use scikit-learn's StandardScaler to scale the features data.

**Part 2: Compile and Evaluate a Model Using a Neural Network**

Use your knowledge of TensorFlow to design a deep neural network model. This model should use the dataset’s features to predict the credit quality of a student based on the features in the dataset. Consider the number of inputs before determining the number of layers that your model will contain or the number of neurons on each layer. Then, compile and fit your model. Finally, evaluate the model to calculate its loss and accuracy.
To do so, complete the following steps:
1. Create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using TensorFlow’s Keras.
2. Compile and fit the model using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric.
3. Evaluate the model using the test data to determine the model’s loss and accuracy.
4. Save and export your model to a keras file, and name the file student_loans.keras.
*NOTE*
Remember to download your saved model from Colab so you can upload it to your GitHub repo.

**Part 3: Predict loan repayment success by using your neural network model**

Use the model you saved in the previous section to make predictions on your reserved testing data.
To do so, complete the following steps:
1. Reload your saved model.
2. Make predictions on the testing data, saving them to a DataFrame and rounding the predictions to binary values.
3. Generate a classification report with the predictions and testing data.

**Part 4: Discuss creating a recommendation system for student loans**

Briefly answer the following questions in the space provided:
1. Describe the data that you would need to collect to build a recommendation system to recommend student loan options for students. Explain why this data would be relevant and appropriate.
2. Based on the data you chose to use in this recommendation system, would your model be using collaborative filtering, content-based filtering, or context-based filtering? Justify why the data you 3. selected would be suitable for your choice of filtering method.
3. Describe two real-world challenges that you would take into consideration while building a recommendation system for student loans. Explain why these challenges would be of concern for a student loan recommendation system.
