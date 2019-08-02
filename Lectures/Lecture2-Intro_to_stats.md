1. What are statistics?
	a. Ask the students. What do they think statistics are?
		i. Write their answers on the board

	b. Definitions from books
		i. "Statistics provide standards of empirical proof" - Ramsey and Schaffer
		
		ii. "How best to collect, analyze, and draw conclusions from data" - Diez et al.
		
		iii. A way to discriminate between variation that is "background" and variation that is "scientifically interesting" - Crawley
		
		iv. "How much variation do we expect by chance?" - Crawley
		
		v. "Data collection, organization, analysis, interpretation, and presentation" - Wikipedia
			A. This is a functional definition, not a conceptual one

	c. My own definition
		i. The previous definitions emphasize the "conclusions" aspect, the "p-value" chase.

		ii. But statistics is really about estimation. It is "the science of uncertainty".
			A. How do we make inferences about the population from a sample?
				1. Define population - The collection of ALL potential units that we wish to make inferences about
					a. Students at Marquette

					b. College students in general

					c. Plants in Wisconsin

					d. Plants in North America

					e. C. elegans / Drosophila

				2. Define sample - The collection of study units on which we make measurements to infer about the population
					a. Cannot possibly measure every unit in a population (usually). So we have to sample.

					b. Sample and population are interrelated. Our desired population should influence our sampling design, but often our sampling design is constrained by logistics, and so our samples dictate the population.
						i. Sampling and experimental design is a whole course unto itself. Quinn and Keough do an excellent job of covering this.

					c. Have to think very critically about the connection between samples and populations when interpreting your results. How general are you conclusions? What populations can you draw inferences about?

2. Basic statistics
	a. Exercise - Weights of candy in a bag from Gelman
		i. Fill a bag with 100 candies of different sizes

		ii. Have students weigh five candies

		iii. Multiply that by 20 to get the full weight of the bag (whoever is closest wins the bag)

		iv. This happens while I'm lecture

	b. What we want to know is how to characterize the "population" from the "sample"
		i. Ask the students - What is the population? What is the sample?

		ii. Ask the students - What quantities do we want to know about the population?

	c. Central tendancy: mean
		i. Provide the formula

		ii. Introduce summation notation

	d. Spread of individuals: standard deviation
		i. Provide formula

	e. Now write the data from the students on the board. Compare to the true weight.
		i. Is there variation among the student's estimates? Why?

	f. Uncertainty of the parameter: standard error
		i. When we measure a sample, that measurement differs among samples. So the measurement itself has error. This is called the "sampling distribution" and is represented by the standard error
			A. Example of the candies (SE of the total weight)

			B. Example of height of Marquette students (average)

			C. Other examples

		ii. The root-n rule: information increase proportional to root-n
			A. Ask the students how they think information is gained from additional samples

			B. Introduce the root-n idea, draw the graph on the board

			C. Discuss the practical implications of the root-n rule.


3. Distributions
	a. Distributions characterize the "shape" of data

	b. Normal distribution
		i. Draw on board

		ii. Mean

		iii. SD
			A. Talk about +/- 1 SD being 68% and +/- 2 SD being 95%

		iv. Confidence interval
			A. What does a confidence interval truly mean?

	c. t-distribution
		i. Draw on board

		ii. The normal assumes we know the standard deviation, but we have to estimate that from the data too. So SD is uncertain as well.
			A. Demonstrate on the board that both the location and the spread are uncertain

			B. The t-distribution allows for the spread to be uncertain by fattening the tails

			C. Parameters
				1. Mean

				2. SD

				3. df.
					a. What are degrees of freedom?

					b. Typically lose one df. per parameter
						i. Explain this for the mean

4. One sample t-test
	a. The goal is to test whether the mean if equal to a certain number (call it H0)

	b. Introduction the notation
		i. y_i ~ t(mu, sigma_y, df)

	c. We want to know if mu = H0

	d. One-tailed vs. two-tailed
		i. In terms of the 95% CI

		ii. We generally say mu != H0 if there is <= 5% chance
			A. Draw the graph

		iii. But we didn't specify whether H0 was bigger or larger, just that it was different
			A. Draw the graph, relate to the 95% CI
				1. On repeated sampling, we would see values in the shaded region only 5% of the time
				
				2. Alternatively, on any given single sample (which is what we usually do), there is only a 5% chance of observing a mean in the shaded regions. 

				3. Thus, any value in the shaded region is "implausible" given the data.

				4. This relates to p-values, but the 95% CI is more informative
					a. Why?

					b. p-values are one number, they say nothing about the effect size or the uncertainty

		iv. Note that this is a null hypothesis test. It is generally not interesting to know if mu is precisely equal to H0 (when would it ever be??). Rather, we are more interested in by how much mu differs from H0, and how certain we are of mu. This is where the effect size and uncertainty come in.
