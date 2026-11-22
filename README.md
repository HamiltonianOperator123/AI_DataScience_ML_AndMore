Hello! I am a student eager to learn and explore Machine Learning and Data structures and its applications in the field of Materials Engineering.
To start off, Linear Regression is a very simple algorithm (a fundamental to AI) that helps in predicting the next estimate datapoint, when we are given a number of datapoints following an almost linear trend.

Where Linear Regression is used:
1. Most engineers must have already experienced plotting graphs of straight lines in physics lab, conducting experiments,
   especially when the working formula behind the experiment has a direct proportionality relation between the dependent and independent variables
2. There will always be some slight uncertainity/error in the measured values, and observations (data points) may thus not always lie on a straight line even when the relation says otherwise. 
3. The more observations (data points) we have, the better estimate of the equation (and thus the slope and offset) that dictates the relationship. We reduce errors by taking more datapoints
4. we can thus predict/estimate the corresponding abscissa (dependent variable) value when given the ordinate(independent variable) value and vice versa.


How it works and its derivation:
-
consider we have set of datapoints (x1,y1),(x2,y2)....(xn,yn). We want to find a line such that the sum of squares as shown in the image <img width="630" height="584" alt="image" src="https://github.com/user-attachments/assets/b20180c2-ecae-4ba7-bec9-230674a09439" />
is minimum. The predicted line need not pass through all or any of the data points, but it will definitely pass throu
Why do we minimize the squares of deviations and not the modulus of the deviations? We do so because of two main reasons:
1. There can be two distinct lines of different slopes and offsets that may have the same value of minimized modulus of deviations,
   but there is only one unique line such that the square of deviations is minimum. This arises from the second reason which is given below
2. The Modulus function is inherently a non-differentiable function. Thus, differentiating it and equating it to zero to find its minima is not possible across its domain.
   but this is not the case with minimizing the square of deviations.    
 
-
DERIVATION:
Let the line which is to be predicted be y=A+Bx (where A is the offset and B is the slope). We basically need to find A and B
we have a collection of datapoints (x1,y1),(x2,y2)....(xn,yn). Area of a square formed by the point (xi,yi) and the line is given by (yi-A-Bxi)^2
the derivation is in this pdf:
[linear regression derivation.pdf](https://github.com/user-attachments/files/35237475/linear.regression.derivation.pdf)













