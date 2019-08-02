1. How do we actually estimate parameters?
	a. Repeat the t-test example
		i. Ask the students to repeat the example (ask them to repeat and explain the notation)

		ii. y_i ~ t(mu, sd_y, nu)
			A. Which parameters are known? Which do we have to estimate?

	b. Let's go back to the normal distribution
		ii. y_i ~ normal(mu, sd_y)
			A. Which parameters are known? Which do we have to estimate?

	c. Normal CDF
		i. Draw the normal curve

		ii. Write the equation that describes the curve
			A. 1/sigma*sqrt(2pi) * exp(-0.5 * (y_i - mu)^2/ sigma^2)

		iii. Since mu and sigma determine the shape of the curve, we are asking "which mu and sigma provide the curve that best fits our data"
			A. That is, we are asking "what is the likelihood of mu and sigma, given the data". L(mu,sigma|y)

	d. Example with one point
		i. Assume we know mu and sigma.
			A. Calculate the likelihood of a single point.

			B. Calculate the likelihood of two points. They are multiplied together to get the likelihood of both points jointly
				1. Discuss the rules of probability. The probability of anything AND anything is the product.
					a. Example: the probability of brown hair AND blue eyes

				2. So how do we get the probability of y1 AND y2?


				3. Introduce product notation
					a. Rules of logs: summation of logs. This is why its computationally faster to add. And easier to minimize than maximize.

		ii. Now go the other direction, which is what we are usually doing. Provide data, and try to estimate mu and sigma.
			A. We want the combination of mu and sigma for which the likelihood is the highest.

			B. Ask the students for guesses. Have them calculate the likelihood.
				1. Is this number informative on its own? Why or why not?

				2. For computational reasons, we often minimize the negative log likelihood. Convert the likelihood to the NLL.

			C. Ask the students for new guesses.
				1. Put a table on the board with four columns: mean, SD, L, NLL

				2. Ask the students to each fill out guesses for mean and SD just by looking at the data.

				3. Calculate the L and NLL together for each one.

				4. Whichever student is closest gets more candy

			D. For a normal distribution, the arithmetic mean and SD are the best estimates of mu and sigma. 
				1. Calculate L and NLL for the arithmetic mean and SD

				2. But as we'll see, it doesn't work for more complicated models. This is a general form of how maximum likelihood works




