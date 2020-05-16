# ML

## Introduction
- What is ML ?
- Why is ML important ?
- Applications of ML.


## Defining an ML problem
Tom Mitchell's Def'n


## Terms
1. Supervised v/s Unsupervised
2. Classification v/s Prediction
3. Overfitting v/s Underfitting



## Optimization Methods
1. Gradient Descent


## Algorithms

1. Linear Regression
2. Logistic Regression
3. Naive Bayes
4. Decision Trees - ID3
5. Artificial Neural Networks
6. Support Vector Machines
7. K means


### Linear Regression
- A prediction algorithm - i.e. output is a real number.
- A very simple but effective model.
- Assumes that the output `Y` depends linearly on the input variables `x_1, ..., x_n`.

#### Training a model
- The model is given by

    `Y = Beta_0 + Beta_1 * x_1 + ... + Beta_n * x_n + e` where

    - `Y` is the dependent variable which will be predicted later on.
    - `x_1, ..., x_n` are the input variables.
    - `Beta_0, ..., Beta_n` are the parameters of regression.
- Define error as Residual Sum of Squares (RSS).

    `error = (e_1)^2 + ... + (e_n)^2` where

    `e_i = Y_i - Y(x_1, ..., x_n)`
- Objective: Find `Beta_0, ..., Beta_n` such that error is minimum.

#### Prediction
- Plug in the values of `x_1, ..., x_n` into the model.
- The predicted value of `Y`, called `YHat` is given by

    `YHat = Beta_0 + Beta_1 * x_1 + ... + Beta_n * x_n`
    
### Logistic Regression
- A Classification algorithm - i.e. output is a class.
- Finds probabilities of belonging to a particular class.
- Creates a "Decision Boundary".

#### Why not use Linear Regression ?
- Linear regression might be used by assigning each class a numerical value, for eg, `yes = 1` and `no = 0`. Predict Yes if `YHat >= 0.5`.
- Works well for cases where `Y` has 2 outcomes.
- However, it might produce probabilities < 0 or > 1.
- Might result in overfitting.
- Not all classes can be accurately represented as numbers.

#### Training a model
- given by,

    `p(x) = e^( Beta_0 + ... + Beta_n * x_n ) /( 1 + e^( Beta_0 + ... + Beta_n * x_n ) ) ` where
    - e = 2.71828 ( approximately )
- `0 < p(x) < 1`

### Naive Bayes

### Decision Trees - ID3

### Artifical Neural Networks

### Support Vector Machines

### K means



## Testing & Improving Accuracy
    Cross validation
    Regularisation
    Feature Scaling

## Conclusion
