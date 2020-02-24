# Predict-Breast-Cancer-malignant-or-benign-using-SVM

We have used the **Support Vector Machine(SVM)** model on the built-in dataset for breast cancer.The prediction that we want to do as far as the class is whether the tumor for this breast cancer is *malignant* or *benign*. There are a bunch of different data points here such as the smoothness of the cancer or the tumor or how compact i.e. the perimeter or the area etc.. There are a total of 30 columns, the details for which can be observed as follows.

Major attributes' information:
- radius (mean of distances from center to points on the perimeter)
- texture (standard deviation of gray-scale values)
- perimeter
- area
- smoothness (local variation in radius lengths)
- compactness (perimeter^2 / area - 1.0)
- concavity (severity of concave portions of the contour)
- concave points (number of concave portions of the contour)
- symmetry 
- fractal dimension ("coastline approximation" - 1)

The mean, standard error, and "worst" or largest (mean of the three largest values) of these features were computed for each image, resulting in 30 features.

Exploratory Data Analysis is performed visually using **seaborn** by create a jointplot between *mean smoothness* and *mean concavity* and plotting all the variables against each other using pairplot.

A SVC classifier and a Grid Search classifier model are created and then predictions are made with each for the test data.

Then the model performance is evaluated by calculating the Classification Report and Confusion matrix for each.

To conclude, the Grid Search classifier model performs tremendously well i.e. *approx. 95%* accuracy as it selects the *best parameters* and thus the *best estimator*. It improved *approx. 30%* accuracy here than by using the simple SVC.
