Topics I need to cover
1. Comparing two groups
2. Linear regression
	a) what is it?
	b) assumptions
	c) checking assumptions
	d) relaxing assumptions
3. Linear algebra
4. Multiple regression
	a) normal way
	b) LA way
5. One-way ANOVA
	a) comparison of two groups
		i. the "normal" way
		ii. the dummy-coding, linear model way
		iii. checking assumptions
		iv. relaxing assumptions
	b) comparison of more than two groups
		i. the "normal" way
		ii. the dummy-coding, linear model way
		iii. the batch coefficients way
		iv. multiple comparisons
6. ANCOVA
7. Two-way ANOVA
	a) the "normal" way
	b) the dummy-coding, linear model way
	c) the batch coefficients way
	d) multiple comparisons
8. Hierarchical models
	a) what they are
	b) repeated measures
	c) random intercept
	d) random intercept + random slope
9. Logistic regression
10. Poisson regression

Additional topics to consider:
1. Information criteria***
2. Multivariate

Need to find a way to potentially use a screen to display graphs when needed. Maybe a projector right on to the white board? Can then draw overtop the graphs if needed

What about CoCALC?

## Week 1

### Lecture Day
1. Introduction
	a) Who I am
	b) What the course is
		i. The idea is to learn statistics (obviously)
		ii. No "cookbook" approach of stepping through textbooks.
		iii. No theorems or analytical proofs
		iv. Instead, will learn linear models. Everything done via simulation
		v. Computational, rather than analytical, approach. Using Python and PySTAN
		vi. We can't cover it all. Just the basics. Going to "go slow". Hopefully give you the tools you need to understand textbooks and more advanced materials when you need them.
			A. Using 'Bayesian' software but not discussing 'Bayesian' analyses because no priors
			B. So everything we're doing is really 'frequentist' statistics (don't confuse that)
	c) Materials
		i. No required books
		ii. Recommended books
			A. Quinn and Keogh - Experimental Design
			B. Draper and Smith - Applied Regression
			C. Ramsey and Schafer - Statistical Sleuth
			D. Gelman and Hill - Applied regression and multilevel models
		iii. Laptop
	d) Survey
		i. Prior stats experience?
		ii. Prior programming experience?
		iii. Will pretend no one has any
	e) Format
		i. One lecture day (1 hour)
			A. No powerpoints, stats can't be taught using powerpoint
		ii. One computer "lab" day (2 hours)
			A. Hands on practice with programming and stats
			B. Will also cover some new material because 1 lecture hours isn't enough. There will be a lot of learning on your own.
			C. There will be a LOT of repetition
	f) Grading
		i. No tests or midterms (test memorization, not learning)
		ii. The key to learning is practice, practice, practice
		iii. Weekly lab exercises (given on lab day, to be turned in by the next lecture)
			A. This will be detailed (like I said, might include new material: both stats and programming)
			B. These can be started in class, I will be there to help.
			C. Can come to me for office hours
			D. Distributed via github. Turn the notebook in to me digitally.
		iv. Weekly quizzes (given on lecture day, to be turned in by next lab)
			A. Will be short, often one or two detailed analysis questions. Only on previous material
			B. Distributed via github. Turn the quiz in digitially.
		v. By design (and by nature), stats education is cumulative. You need to show up every week and do the work every week to understand what goes on the next week.
	g) Final project
		i. Analyze real datasets to ask real questions
			A. Can use your own data (talk to me first)
			B. I'm happy to provide data for those that don't have it

2. Getting the Anaconda Python environment set up
	a) Download Anaconda and install
		i. Make sure hit 'yes' on the path
		ii. Run 'python' from the terminal, check for Anaconda
		iii. conda-forge
		iv. update all packages
		v. install PyStan
			A. special instructions for Windows?
	b) IDE
		i. Show mine (sublime + terminal)
		ii. Spyder
		iii. Atom
		iv. PyCharm
		v. Visual Studio
		vi. Google Python IDE and pick yours!
		vii. Jupyter notebook

### Lab Day
1. Introduction to Python (NEED TO READ SOME INTRO TO PYTHON BOOKS HERE)
	a) Python is a calculator
	b) Objects
	c) Attributes and methods
	d) for loops
		i. regular
		ii. nested
	e) Modules
	f) Graphics
		i. Graphics are a good way to start here
		ii. Graph some distributions






## Week 2

### Lecture Day
1. What are statistics?
	a) Definitions from books
		i. "statistics provides standards of empirical proof" - Ramsey and Schaffer
		ii. "how best to collect, analyze, and draw conclusions from data" - Diez et al
		iii. a way to discriminate between variation that is "background" and variation that is "scientifically interesting" - Crawley
		iv. "how much variation do we expect by chance?" - Crawley
		v. "data collection, organization, analysis, interpretation, and presentation" - Wikipedia
	b) My own definition
		i. These previous definitions emphasize the 'conclusions' part, the 'p-value' chase.
		ii. But statistics is really about estimation: "The science of uncertainty"
			A. extrapolating from samples to populations
			B. Define POPULATION
			C. Define SAMPLE	
		
2. Basic statistical quantities
	a) Exercise
		i. The weights of candy in a bag from Gelman
			A. Fill a bag with 100 candies of different sizes
			B. Have each student estimate the weight of five candies
			C. Multiply that by 20 to get the full weight of the bag.
			D. This happens while I'm lecturing
	b) How can we characterize the "population" from this "sample"?
	c) Central tendancy: Mean
	c) Spread of individuals: Standard deviation
	d) Compare the candy estimated weights to the 'true' weight
		i. Do they differ? If so, why?
	e) Uncertainty of the mean: Standard error
		i. The root-n rule: information increases with at a root-n rate
		ii. Discuss the importance of the root-n rule

3. Distributions
	a) Distributions characterize the "shape" of a population; the spread of the data
	b) Normal distribution
		i. Mean
		ii. SD
		iii. Confidence interval
			A. What does a confidence interval truly mean?
	c) t-distribution
		i. Accounts for uncertainty in sigma

4. One sample t-test
	a) Introduce the i notation
		i. y_i ~ t(mu, sd_y, nu)
		ii. What is a degree of freedom?
			A. Example with the mean
			B. Example with the variance
			C. Typically lose one degree of freedom for every parameter we are estimating
	b) One-tailed
	c) Two-tailed




### Lab Day




## Week 3

### Lecture Day
1. Parameter Estimation

## Week 4

### Lecture Day
1. Linear regression
	a) Objectives of regression
		i. Two quantitative variables
			A. FIND AN EXAMPLE
		ii. Determine whether or not a relationship exists between the two variables
		iii. Describe the mathematical form of the relationship
		iv. Predict new values (and assess the accuracy of those predictions)
	b) Show scatter plot (NEED EXAMPLE)	
		i. Need to fit a line through these points
		ii. Class example from the Gelman book. Have students estimate their own line. Then estimate the means at each x and estimate the line from that. Compute the sum of squared errors (using a ruler). Compare.
	c) Show the equation for a line
		i. y = B0 + B1 X
		ii. What do these equations mean?
			A. Interpretation of B0 and B1
			B. Give multiple examples
	d) How is the line fit?
		i. Maximum
	e) Show the different formulations
		i. B0 + B1 X doesn't fit the line perfectly, there is scatter around it
			A. y_i = B0 + B1 x_i + e; e ~ N(0, sigma_y)
		ii. B0 + B1 X gives the predicted value, yhat
			A. yhat_i = B0 + B1 x_i; y ~ N(yhat, sigma_y)
		iii. The equations are read as "mean value of y for a given value of x, with the observed value being noisily distributed around the mean"
			A. There are many reasons the noise term exists
				1. Unmeasured variables
				2. Measurement error
				3. Imperfect information
		iv. The linear model (for this and ALL other examples through the course) are not the truth: there are many models that can describe the mean, we are simply looking at one possible model.
	f) Assumptions
		i. Independence
		ii. Heteroscedasticity
		iii. Normality
			A. Normality of the ERRORS, not the data
		iv. Linearity
		v. X is fixed, measured without error
			A. This means repeated sampling would generate the same X's
			B. We can relax this assumption easily in STAN
	g) Accuracy of the predictions
		i. Residual error
			A. Regular residuals
			B. Standardized residuals
		ii. R2
	h) Covariance of parameters
		i. The line always goes through the mean (bar{x}, bar{y}).
		ii. This constrain imposes covariation on the parameters
			A. Show graphically




### Lab Day
1. Linear regression
	a) Make a scatter plot
	b) Fit a model step-by-step
		i. Fit the model
		ii. Calculate R2 (within the model)
		iii. Check assumptions
			A. Normality of errors (QQ plots)
			B. Constant variances (residuals vs fitted)
		iv. Validate accuracy
		v. Assess "significance"/effect size: means, CIs
		vi. Plot results
			A. Coefficient plots
				1. Scatter plot of parameters to show covariance
				2. Marginal histograms
				3. 95% CI plots
			B. Scatter plots
	c) Relax assumptions
		i. Make a scatter plot where variances clearly increase
		ii. Fit the model again
			A. This time, use different variance formulas
			B. Check assumptions


## Week 5



### Lecture Day
1. Linear algebra
	a) Addition
	b) Subtraction
	c) Vector multiplication
	d) Matrix multiplication

2. Linear algebra form of regression
	a) Design matrix
	b) Vector of coefficients

3. Transformations
	a) Standardization
		i. Why do it?
			A. Computational stability
			B. Other advantages in multiple regression that we'll talk about later
		ii. What does this do to the coefficients?
		iii. In general, I do this every time
	b) Log-y
		i. Why do it?
			A. Show the equation
			B. Stabilizes variances (they become multiplicative)
			C. But also changes functional form
		ii. Changes the functional form of the relationship
		iii. Useful when data vary over orders of magnitude (brain size / body weight example)


### Lab Day
1. Linear regression again
	a) This time in linear algebra form
	b) Go through the whole process again (repetition, repetition)

2. Transformations
	a) Examples of transformations
	b) Covariance plots of standardized coefficients



## Week 6



### Lecture Day
1. Multiple regression
	a) Objectives
		i. Assess the effects of multiple predictors on the response
		ii. Assess the effect of one predictor while controlling for confounding variables
			A. People often say all predictors have to be independent.
			B. This is untrue. If all predictors are independent, just do a series of linear regressions. MR is specifically for isolating effects among correlated predictors.
	b) Show the equation
		i. Multiple forms
			A. y_i = B0 + B1 x1_i + B2 x2_i + e; e ~ N(0, sigma_y)
			B. yhat_i = B0 + B1 x1_i + B2 x2_i; y ~ N(yhat, sigma_y)
			C. yhat = XB; y ~ N(yhat, sigma_y)
				1. This is the preferred form because it generalizes to as many predictors as needed
		ii. Brain size example
			A. the equation is "mean brain size for given values of X" (see Ramsey and Schaffer)
	c) Interpreting parameters
		i. In a two predictor case, the parameters describe a plane
			A. Draw the plane
			B. The parameters are the effect of adding 1 to the predictor while holding the other constant
		ii. Brain size example
			A. I like Ramsey and Schaffer's comparison of linear to multiple regression (the last part of Chapter 9.2)
	d) Assumptions
		i. Same as for linear regression
	e) Goodness of fit
		i. Talk about R2
			A. R2 always goes up as parameters are added
			B. Need adjusted R2


### Lab Day
1. MR example using brain size
	a) Pairwise scatter plots
	b) Pairwise scatter plots (log-log transforms)
	c) Create the design matrix
	d) Build the model
	e) Fit the model
	f) Check assumptions
	g) Check parameters
		i. Covariance plots
		ii. Marginal plots
		iii. 95%CI plots
	h) Get R2/adjusted R2
2. Add in predictor for brain size
	a) Redo it all
	b) Compare R2/adjusted R2/parameter estimates from previous model 



Significance of parameter depends on what other parameters are included? Why?
	This is better for a quiz




## Week 7

### Lecture Day
1. Multiple regression odds and ends
	a) Partial plots/added variable plots
	b) Collinearity
		i. What is collinearity?
		ii. How do we assess it?
		iii. What problems does it cause?
			A. Can't interpret parameter estimates: strong relationships but no significance
	c) Standardization
		i. This helps parameter interpretation
	d) Interactions
		i. Quadratic terms as a special case of interactions
		ii. Should always include 'main effects' when including interactions



### Lab Day




## Week 8

### Lecture Day
Dummy variables: echolocation example from Ramsey and Schaffer

### Lab Day




## Week 9

### Lecture Day

### Lab Day




## Week 10

### Lecture Day

### Lab Day




## Week 11

### Lecture Day

### Lab Day




## Week 12

### Lecture Day

### Lab Day




## Week 13

### Lecture Day

### Lab Day




## Week 14

### Lecture Day

### Lab Day




## Week 16

### Lecture Day

### Lab Day

