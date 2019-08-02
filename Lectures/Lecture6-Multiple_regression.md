1. Objectives
	a. Assess the effects of multiple predictors on the response
		i. Useful when many possible factors influence an outcome

		ii. EXAMPLES

	b. Assess the effect of one predictor while controlling for confounding variables
		i. Useful when the effect of one predictor is unknown, but others are known

		ii. People say predictors have to be independent. This is untrue. If all predictors are independent, we can mathematically prove that the answers would be identical for separate single linear regressions. The strength of MR is for isolating effects among correlated predictors.

2. Show the equation
	a. y_i = b0 + b1 x1_i + b2 x2_i + ... + bk xk_i + e; e ~ normal(0, sigma_y)

	b. yhat_i = b0 + b1 x1_i + b2 x2_i + ... + bk xk_i; y ~ normal(yhat, sigma_y)

	c. yhat = Xb; y ~ normal(yhat, sigma_y)
		i. This form is preferred because it generalizes to k predictors

		ii. Show the design matrix formulation (actually write it out)

	d. Brain size example from Ramsey and Schaffer
		i. Show the equation in words

		ii. Put the equation into the design matrix and coefficient vector

		iii. The equation is "mean brain size for given values of X", or mu | X (see Ramsey and Schaffer)

3. Interpreting parameters
	a. In a two predictor case, the parameters describe a plane
		i. Draw the plane

		ii. Parameters are the effect of adding 1 to the predictor while holding the other constant
			A. Talk about this in context of the brain size example (see the last part of Chpt. 9.2 in Ramsey and Schaffer)

			B. Connect this to the objectives. This is the power of MR, to isolate effects

4. Assumptions
	a. Same as for single linear regression, but go over them again

5. Goodness of fit
	a. R2 always goes up as parameters are added, even if they are useless

	b. Need the adjusted R2, which penalizes R2 for the number of parameters

6. Model selection
	a. How do we choose which parameters are "significant", to keep them in the final model?
		i. In this simply case, we can simply look at which parameters have strong effects or low uncertainty (i.e. which parameters have 95% CI that do not overlap zero)

	b. How do we distinguish among multiple competing hypotheses?

	b. BAD - Do not compare R2 among all possible models

	c. GOOD - Use the full model only, just talk about which parameters were significant

	d. GREAT - Use model selection criteria to distinguish among competing hypotheses

7. AIC

	a. Assume you have multiple working hypotheses (not an ALL subsets approach)

		i. EXAMPLE??

	
