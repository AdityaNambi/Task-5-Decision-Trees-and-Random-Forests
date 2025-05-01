# Task-5-Decision-Trees-and-Random-Forests
Tree-based models for classification &amp; regression.

1.Load the Dataset
The CSV file (heart.csv) is loaded using pandas. The dataset contains features related to patient health and a target variable indicating heart disease presence.

2.Prepare Features and Target
The target column (target) is separated from the feature columns (X), and the data is split into training and testing sets (70% train, 30% test).

3.Train a Decision Tree Classifier
A basic DecisionTreeClassifier is trained on the training data. This forms the baseline model.

4.Visualize the Decision Tree
The trained tree is exported using export_graphviz and rendered with Graphviz. This generates a .pdf file showing the decision structure with splits and leaf nodes.

5.Analyze Overfitting by Tree Depth
Multiple Decision Trees are trained with varying max_depth (from 1 to 20). Their training and testing accuracy are plotted to understand how tree depth affects overfitting and underfitting.

6.Train a Random Forest Classifier
A RandomForestClassifier is trained using the same training data. Predictions are made on the test set, and accuracy is printed to compare with the single Decision Tree.

7.Interpret Feature Importances
Feature importances are extracted from the Random Forest model and visualized using a horizontal bar chart to identify which features most influence predictions.

8.Evaluate with Cross-Validation
Both models are evaluated using 5-fold cross-validation. The mean accuracy and standard deviation across folds are printed for both Decision Tree and Random Forest, providing a more robust performance measure.
