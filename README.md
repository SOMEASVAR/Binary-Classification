# BINARY CLASSIFICATION
## Aim:
To write a python program to perform binary classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner /Google Colab

## Related Theoritical Concept:
```
1.numpy-used to manipulate arrays and mathematical operations on arrays. 
2.matplotlib.pyplot as plt-used to represent the given data set in a 
graphical manner. 
3.sklearn-used for statistical modelling and build machine learning models. 
4.datasets-used to introduce many small datasets and fetch large data sets. 
5.make_blobs-used to generate blobs of points with a gaussian distribution. 
6.counter-It is a sub class of dictionary class used to count the key-value pair in 
the given data set. 

```

## Algorithm
## Step 1: 
Import necessary libraries from packages. 
## Step 2: 
Assign x,y values from the given dataset by sklearn. 
## Step 3: 
Count the number of key-value pairs in the datasets using counter libraries. 
## Step 4: 
Plot the x and y values in the chart using mathplotlib.pyplot 
## Step 5: 
Label the values of x and y axis and add title to the graph . 
## Step 6: 
Save the file and execute the program.

## Program:
```
Program to implement binary classification.
Developed by: R.SOMEASVAR
RegisterNumber:  212221230103
```
```
from numpy import where 
from collections import Counter 
from sklearn.datasets import make_blobs 
from matplotlib import pyplot 
X, y = make_blobs(n_samples=10, centers=2, random_state=1) 
print(X.shape, y.shape) 
counter = Counter(y) 
print(counter) 
for i in range(5): 
 print(X[i], y[i])  
for label, _ in counter.items(): 
 row_ix = where(y == label)[0] 
 pyplot.scatter(X[row_ix, 0], X[row_ix, 1], label=str(label)) 
pyplot.legend() 
pyplot.show() 
```

## Output:
![binary classification plot](1.jpg)


## Result:
Thus the python program performed binary classification successfully.
