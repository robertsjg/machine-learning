Machine Learning Notes

Terminology

Supervised Learning Algorithm

Supervised learning algorithm given data in which told the "correct" answer
Regression problems predict a continuous output value (following quadratic or linear curve) E.g. house value v size

"parametric methods" - two step model based:
					1. Make assumptions about functional form of f e.g. a linear model 
					2. Apply a procedure to train the model e.g. least squares

"non-parametric methods" - no explicit assumption about f, f is estimated as close to the data points, better fir where the a models "truth" is uncertain, while flexible needs a very large data set to get accuracy, overfitting in this case can make accurate estimates of new observations (not in original data) inaccurate					

"overfitting" - More complex models can lead to a phenomenon known as overfitting the data; following the errors, or noise, too closely

Different statistical methods have trade offs between interpretability and flexibility e.g. least squares is low on flexibility and fairly interpretable 
restrictive methods can be of most use when applied to inference rather than prediction

Training Set -> Learning algorithm -> Hypothesis

Example Supervised Regression Training Set

Size | Price 
2000	100
1400	 85
3000	245
3100	265
800		 50

m = no training samples (5) 
x = input variables/features
y = output/target variable

Example Supervised Regression Hypothesis

new size (x) -> hypothesis (h)  -> new estimated price (y)
so h maps x's to y's

Cost function
## θ (theta)
hθ(x) = θ0 + θ1x1 + θ2x1
make hθ(x) close to y for training samples

Matrix multiplication 

Scalar multiplication 2 * [4 0 2 -10] = [8 0 4 -20]
Matrix * Matrix uses the "dot product" of rows and columns, take first row an multiply by first column  

In Python the numpy or sympy package has a matrix collection (or arrays for speed)



Classification problems result in discrete output values (E.g. 0 or 1, positive or negative)
Features - E.g. when trying to determine if a tumour is benign or malignant features would be - size, age, clumpiness, shape, etc.  

Unsupervised Learning Algorithm

Unsupervised learning algorithm given unstructured data, find patterns E.g. grouping news articles about the same story, given customer data discover market segments understand the relationships between the variables or between the observations

Methodology - cluster analysis, creating groups based on observations
