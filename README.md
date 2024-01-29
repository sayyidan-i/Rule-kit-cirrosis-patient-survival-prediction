This notebook focuses on building a predictive model for cirrhosis patient survival using the RuleKit package for fuzzy inference system and classification tasks. The code is structured into different sections for clarity and ease of understanding.

## Importing Packages
- RuleKit is installed using the command `!pip install rulekit`, and its required JAR file is downloaded.
- Additional packages such as pandas, numpy, rulekit, RuleClassifier, and sklearn metrics are imported for data manipulation, model training, and evaluation.

## Importing Dataset
- The `ucimlrepo` package is used to fetch a cirrhosis patient survival prediction dataset.
- The dataset is loaded into pandas dataframes for features (`X`) and targets (`y`).

## Preprocessing Data
- Data preprocessing steps include dropping rows with null values, changing data types of certain columns, and flattening the target variable.
- The columns 'Cholesterol', 'Copper', 'Tryglicerides', and 'Platelets' are converted to numeric data types, and rows with NaN values in these columns are removed.

## RuleKit Initialization and Model Fitting
- RuleKit is initialized using `RuleKit.init()`.
- A `RuleClassifier` is created, and the model is fitted using the provided features (`X`) and targets (`y`).

## Displaying Rules
- The rules obtained from the trained RuleKit model are printed.

## Predictions and Evaluation
- The model is used to predict the target variable on the same dataset (`X`).
- Accuracy, F1 score, and a confusion matrix are computed and displayed.

## Simulation with User Input
- The code simulates a system by taking user input for patient information.
- The trained RuleKit model is used to predict the patient's class (Cencored, Cencored due to Liver Transplantation, or Death).
- The predicted class is then printed for the user.

Feel free to use this notebook as a reference for building fuzzy inference systems with RuleKit for classification tasks, especially in the context of cirrhosis patient survival prediction. The provided simulation section allows users to interactively input new data and observe the model's predictions.
