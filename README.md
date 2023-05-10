# Neural_Networks
Multiple neural network models are used and evaluated for breast cancer detection and prediction in a classification supervised learning environment.

## Libaries
The following python libraries were used:
* _pandas_ - for use in creating and manipulating dataset using dataframe
* _numpy_ - used for numerical calculations
* _matplotlib_ - plot generation
* _seaborn_ - plot generation
* _sklearn_ - for splitting training and test sets, implementing logistic regression, creating confusion matrix and classification report, precision-recall curves, and calculating accuracy
* _tensorflow_ - open-source libary used to create neural network, adjust hyperparameters, and evaluate performance

## Project Motivation
The project motivation was to use a publicly available dataset in order to explain the underpinnings of neural network models - from neural network structure, how model predictions are computed, and performance comparisons using multiple metrics of evaluation of accuracy and precision-recall curves. Pros and cons of each model are discussed, key takewaways are listed, and follow-up questions for further research are presented.

The Medium blog post explaining this can be found at the following link:  
https://rbernas.medium.com/breast-cancer-detection-using-neural-networks-3eebf492758d

## Files
* _Neural Network Models.ipynb_ - Python source code 
* _breast-cancer-wisconsin.data_ - Dataset 
* _breast-cancer-wisconsin.names_ - Dataset readme file

## Analysis Summary
Three neural network models were presented. One model was a logistic regression model, while the other 2 models were dense neural networks with varying hyperparameters. The logistic regression model worked well, considering the much lower complexity and computational cost compared to the neural networks. This was primarily because the dataset was largely linearly separable and shown during exploratory data analysis. For all three models, 4 separate metrics of evaluation were shown - accuracy, precision, recall, and break-even points - in order to be mathematically precise in supporting the claim that one model performance was better than the other. Overfitting was presented in one of the neural network models, showing the decrease in performance on the test set. Because of this, the logistic regression model performed better, though not as well as the second neural network model. This was because the second neural network model was able to capture the slight non-linearities in the dataset due to the use of activation functions, at the cost of added complexity and computational resources.    

## Acknowledgments 
This breast cancer databases was obtained from the University of Wisconsin Hospitals, Madison from Dr. William H. Wolberg, and publicly available online via the University of California, Irvine (UCI) Machine Learning Repository website (https://archive.ics.uci.edu/ml/index.php). Additional people who worked on the database are listed below:

   1. O. L. Mangasarian and W. H. Wolberg: "Cancer diagnosis via linear 
      programming", SIAM News, Volume 23, Number 5, September 1990, pp 1 & 18.

   2. William H. Wolberg and O.L. Mangasarian: "Multisurface method of 
      pattern separation for medical diagnosis applied to breast cytology", 
      Proceedings of the National Academy of Sciences, U.S.A., Volume 87, 
      December 1990, pp 9193-9196.

   3. O. L. Mangasarian, R. Setiono, and W.H. Wolberg: "Pattern recognition 
      via linear programming: Theory and application to medical diagnosis", 
      in: "Large-scale numerical optimization", Thomas F. Coleman and Yuying
      Li, editors, SIAM Publications, Philadelphia 1990, pp 22-30.

   4. K. P. Bennett & O. L. Mangasarian: "Robust linear programming 
      discrimination of two linearly inseparable sets", Optimization Methods
      and Software 1, 1992, 23-34 (Gordon & Breach Science Publishers).

