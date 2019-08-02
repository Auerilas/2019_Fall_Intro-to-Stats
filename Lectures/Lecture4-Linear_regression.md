1. Objectives of regression
	a. Present an example of two quantitative variables (NEED EXAMPLE)
		i. Define PREDICTORS and RESPONSE variables

	b. Determine whether or not a relationship exists between the two variables

	c. Describe the mathematical form of the relationship

	d. Predict new values of the response from the predictors

2. Conceptual example
	a. Show a scatter plot of the quantitative variables
		i. Need to fit a line through these points

		ii. Class example from the Gelman book. Have students estimate their own line. Have students draw their lines on the board.
			A. For each line, show the errors.

			B. Calculate the MSE as a measure of fit for each stduent (using a ruler)

			C. Then, draw a line based on the mean of y at each x and calculate MSE for that

	b. Show the equation for the line
		i. y = b0 + b1x

		ii. What do these parameters mean?
			A. Interpretation of b0 and b1

	c. b0 + b1x doesn't fit the data perfectly, there is scatter around it
		i. y_i = b0 + b1x_i + e_i; e ~ normal(0, sigma_y)
			A. Explain this equation

		ii. yhat_i = b0 + b1x_i; y ~ normal(yhat, sigma_y)
			A. Maximum likelihood notation
				1. mu = b0 + b1x; sigma = sigma_y
				
				2. Insert this into the normal PDF
				
				3. L(b0, b1, sigma_y | y)
					a. We are going to trust our software to find the parameter combinations that maximize the liklihood

		iii. These equations are, in words, "the mean of y for for a given value of x, with the observed data being noisily distributed around the mean"
			A. There are many reasons the noise term exists
				1. Unmeasured variables

				2. Measurement error

				3. Imperfect information

		iv. This is a LINEAR model because it is linear in parameters. It is not the truth. There are many models that can describe the mean, it is simply one possible model.

	e. Assumptions (in order of importance)
		i. Independence
			A. Independence is the measurement of one point being unrelated to a measurement of another
				1. Given examples of non-independece (number of plant species in one field, length and weight of C. elegans, size of fish in an aquarium, etc)

		ii. Equality of variance (homogeneity of variance, homoscedasticity)
			A. Show what this means visually. Show how it is integral to the equation, every y_i has the same sigma_y

		iii. Normality of errors
			A. ERORRS, not the DATA

			B. Show how this is in the equation, and what it means visually

		iv. Linearity

		v. X is fixed, measured without error
			A. This means repeated sampling would generate the same X's
				1. Give examples of experiments where this is satisfied

				2. Give examples of experiments where it is not

			B. In practice, we usually ignored this becauseit was complicated to account for measurement error in X. But using STAN, we can (and will) relax this assumption.

3. What are we testing?
	a. Ask the students what the parameters of interest are?

	b. Ask the students what they think we are testing?
		i. Is b1 different from 0?
			A. Ask the students if this is the only relevant question

			B. If b1 is different from 0, shouldn't we be interested by how much and how certain we are of it?
				1. Give examples of significant but irrelevant based on small effect size and/or high uncertainty

4. Accuracy of predictions
	a. What is a residual?
		i. Regular residuals

		ii. Standardized residuals (will be important later when we relax the assumption of equal variances)

	b. MSE (we already discussed)
		i. Show the formula (sum(e^2))

	c. R2
		i. Show the formula

5. Covariance of parameters
	a. The line always goes through the mean (bar(x), bar(y))

	b. This constraint imposes covariation on the parameters
		A. Show graphically
