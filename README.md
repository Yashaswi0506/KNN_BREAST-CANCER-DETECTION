# KNN_BREAST-CANCER-DETECTION

Dataset is an important parameter as the accuracy of the classifier depends on the input data. A good
dataset should be chosen which has many features. In this project we have chosen Breast Cancer
Wisconsin (Original) Data Set . There are 11 features in this dataset along with the classification label.
The labels are classified as 2 and 4 in the dataset where 2 stands for Benign and 4 stands for Malignant.
The dataset has a total 699 rows, out of which 458 rows are benign and 241 are malignant.

K Nearest Neighbours(KNN) is a supervised learning algorithm used for classification and
regression predictive problems. Generally KNN is used for classification. The below two terms
defines KNN in more detail
Lazy Learning algorithm : It is defined as a lazy learning algorithm because it doesn’t learn
anything in the training phase, it just loads the data in the training phase instead it learns in the
testing phase.
Non-parametric learning algorithm : KNN is a non parametric algorithm as it doesn’t consider
any condition about the data.
KNN implementation in breast cancer detection : KNN is based on similarity features. Here
we have two categories for classification i.e., 2 for Benign and 4 for Malignant. We want to
classify what classes the sample of the training data set belongs to. So, by using KNN we will
observe the behavior of the nearest sample from the test data set and classify the train set
accordingly. We are dividing data into training and test data sets. Where training data is 75% and
test data is 25%.
Now the question is how many neighbors to consider, i.e., selecting the value of K?
Value of K :When K = 1, it will overfit by performing well in the training phase but may not
perform well in the testing phase. Another problem is that K is not set as even in binary
classification. Let’s say we have K = 6 and there is a tie between two labels from all 6 neighbor's
votes then there will be a confusion as to which class is to be assigned. Therefore setting the
value of K as an odd number and square root of the total length of the dataset.
Value of K is calculated based on the minimum error. To calculate minimum error euclidean
distance is found between training data set against test data set and prediction is calculated. Then
the predicted labels are compared against test_label and mean of error is calculated. This process
is repeated 10 times and from 10 iterations the least value of K is chosen to get the maximum
accuracy.