# DSAN5000CourseNotes

## Machine Learning Paradigm Overview
### Age and Income
* mathematics used will be similar to those training language models
* learning how to fit a univariate curve
* option instead of a parabola in this case could be a Sigmordal function with a number line
* question is whether or not the data points are stochastic models
* know if deviation in the curve is a "real" effect or statistical effect, to know this you must get more data
* if you get better statistical noise, there will be less variation
### Data Generated Function: Ground Truth 
* a parabola would be the ground truth functional form for a regression
* Data Provenance: tracing data origin, transformations, and changes. Ensures accountability, reliability, and quality in data-driven processes and decisions
* Neural networks tend to entropolate (not fit the data well)
* you need mathematical modeling not curve fitting
* Understand fundamental property of nature
* Good data captures aspects of the ground truth
* Good labeled data is a representation of the ground truth
### Regression Tasks
#### Scalar Regression (or curve fitting)
* intercept, fitting parameter for x1 and x2
* x is a vector and a parameterization
* scalar regression is learning a plane in two dimensions
## Univariate Curve Fitting Example
* parametric model = functional form + parameterization
## What Does This Mean: Parametric Model = Functional Form + Parameterization

In simple terms, a **parametric model** is a type of model in which the structure of the relationship between input and output is defined by a specific mathematical formula (the **functional form**) and relies on a set of values (**parameters**) to make predictions.

### Breaking it Down:
- **Functional Form**: This is like the blueprint or the general shape of the model. For example, a straight line equation like `y = mx + b` is a functional form where `m` and `b` determine the line's slope and intercept, respectively.
- **Parameterization**: These are the actual values of the parameters (e.g., `m` and `b` in the line equation) that the model uses to make specific predictions. The process of finding the best values for these parameters is called **fitting** or **training** the model.

### Putting It Together:
A **parametric model = functional form + parameterization** means that the model first decides on a formula (e.g., linear, polynomial) and then finds the best parameter values to use that formula for making predictions.

For example:
- If you're using a simple linear regression model (`y = mx + b`), the **functional form** is the equation `y = mx + b`, and the **parameters** are `m` (slope) and `b` (intercept).
- The model learns or estimates these parameters (`m` and `b`) from the data to provide the most accurate predictions.

**Key Point**: In parametric models, the number of parameters is fixed, which makes them straightforward but potentially less flexible compared to non-parametric models, which can adapt more to the data without assuming a fixed form.

### Example: Gaussian
* forms a space of all possible functions
* goal in ML is finding a special set of numbers that fit the data
* Goal of machine learning process is to learn the four numbers that fit the data
* To do the above, you can train functions to optimize them to learn the parameters to fit the data
* refer to common parent functions
* depending on the shape of the data visualization or plot, like for example a linear plot, will tell us the function for deep learning
* quadratic function used when the line goes through everything
* if you are fitting a linear function the optimization will occur in r2
* to fit sinusoidal data (a trigonometric function) you'll be doing
* binary classification with a logistic function
* outputs of a linear model will give outputs either 0 or 1 because it has a meaning of a probability

Fourier Series: you don't do optimization in this because they have orthogonality

Neural Network Model: you can write down the analytical expression of a neural network as a function

## Common ML Workflow Summary
* Step 1: Define the problem

* Simple example: distance from some city center, and housing prices
* Getting data: going door to door asking people how much their houses are
* go back make a data frame and make a data table
  
* one input: distance from city center
* one output: price of a house

* Choosing a measure of success
* surveyer one and surveyor two both go different routes
* however, surveyer just sees data, but it is not predictive at all

### Data needs a model

* but first, you must prepare the data
* data can only see local qualitive trends

Solution: coming up with a functional form of the data which will make it easier to choice parameter initial conditions (IC)

* Developing a model that does better than some baseline
* Concept of noise
* when you see data you just see central tendency
* functions are envelope of noise
* minimum and maximum envelope of noise
* Omnipotent: fully predictive and perfectly accurate at all possible X points
* Ideal Data -> Infinite Sampling Capability N -> infinity
* Gaussian processes will give you central tendency and other stuff

* ML are just curve fitters
* if the model can fit the provided data, it will probably interpolate well
* extrapolation, transferability
* concept of whether or not you are inside the data cloud
* test how smart a large language model is

* are large language models truly rational

* scaling up: developing a model that overfits
* regularizing your model and tuning your hyper-parameters

* General Artificial Intelligence: the holy grail of ML???
* this is a model that takes experience and will do what you show it but like we have it with reinforcement learning algorithms but we do not have it
* temporal decision making in very complicated spaces
* whether or not cognition or transferrable --- apple wrote a paper on SAT
* normalize data to have units
* we normalize because it makes it easier to fit data

* location of first gausian vs location of second gaussian

* M(x|P) = Model
* you have to guess

* partition data into three spaces
*   cross validation: data that learns parameter vectors
*   error of validation set, error of test set
*   model must be systematically hyper parameter tuned through cross validation

It is possible to accidentally overfit data through the optimized hyperparameter loop

using a test set inside of your workflow's model is cheating i guess

any time you do ML you have to cross-validate

linear regression gives you a baseline when doing a regression model

Visualizing a 4 dimensional object 

encoding variations in a 3 dimensional space: feedback signal visualized by color

2 parameter model is a 2 dimensional space 

minimum value is the best fit model because it minimizes the RMSE or root mean squared error

special parameter values that minimize the RMSE

## Gradient Based optimization
- goal is to minimize law surface
- gradient descent is how you train models
- most neural networks are trained with parameters of neural network that stand with loss function
- gradient calculation is necessary to train models
- iteratively train a neural network
- gradient descent learning gets a special name
- back propagation to learn gradient vectors so you can train neural network
  
* back propagation computes the gradient vector
* iterative updates of trading process

Special Parameterization 
optimal model minimizes the validation error.

model is the architecture plus parameters

## Invest time in learning calc 3 problem about 
i think the loss function RMSE or AKA the objective function

## Start with an Initial Guess
## Model Training Diagram
* feed it into your parametric model
* ouput an initial set of predictions
* true targets Y
* predictioons Y
* loss function is a single number
