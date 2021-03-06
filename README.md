# Fluoranthene_Detection
UBC Okanagan - ENGR 518 Applied Machine Learning, Group 7  
Yifan Pan, Yirao Zhang, Zhenyu Ma, Xufei Wang

## Requirement
### Python (Done)
```numpy```  
```pandas```  
```matplotlib```
### Matlab (TODO)
For project details, please check pdf file.  

## Dataset Preprocess
Training dataset has ```336``` datapoints with ```29 * 111``` columns.   
Test dataset has ```200``` datapoints with ```29 * 111``` columns.  
For convenience and computing efficiency, we aggregate every 111 columns as 1 column by calculating the mean value. 
Besides, we set a new column as ```ground truth label```, which is produced by checking whether the value of first column is greater or smaller than 0.5 (0 if smaller than 0.5, 1 if greater than 0.5).
For dataset details, please check pdf file. 

## Machine Learning Model
Since this project is a 2-class classification problem, we use ```linear regression model``` to classify datapoints.  
We now implemented ```Sigmoid``` activation function and ```cross-entropy``` cost function.  
We now implemented ```gradient descent``` as our optimization algorithm.

## How to Run
Just run ```LinearTwoClassClassifier.py```.  
This file has whole training and testing body codes.

## Result
Our machine learning model was proved that it has a ```97%``` balanced accuracy on test dataset.  
Our experiment confusion matrix is shown in ```cm.jpg```.

## TODO
1. some bugs when plotting learning curve.  
2. May try Newton method.  
3. May implement this project in Matlab.
