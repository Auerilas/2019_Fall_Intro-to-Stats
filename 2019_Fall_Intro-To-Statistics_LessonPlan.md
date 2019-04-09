Topics I need to cover
1. Correlation (MAYBE??)
2. Linear algebra
2. Linear regression
	a) assumptions
	b) checking assumptions
	c) relaxing assumptions
3. Multiple regression
	a) normal way
	b) LA way
4. One-way ANOVA
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
5. ANCOVA
6. Two-way ANOVA
	a) the "normal" way
	b) the dummy-coding, linear model way
	c) the batch coefficients way
	d) multiple comparisons
7. Hierarchical models
	a) what they are
	b) repeated measures
	c) random intercept
	d) random intercept + random slope
8. Logistic regression
9. Poisson regression

Additional topics to consider:
1. Information criteria
2. Multivariate

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
			A. Draper and Smith - Applied Regression
			B. Ramsey and Schafer - Statistical Sleuth
			C. Gelman and Hill - Applied regression and multilevel models
		iii. Laptop
	d) Survey
		i. Prior stats experience?
		ii. Prior programming experience?
		iii. Will pretend no one has any
	e) Format
		i. It's a 2 credit class, but we'll meet for more than two hours
		ii. One lecture day (1 hour)
			A. No powerpoints, stats can't be taught using powerpoint
		iii. One computer "lab" day (2 hours)
			A. Hands on practice with programming and stats
			B. Will also cover some new material because 1 lecture hours isn't enough
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
			A. special instructions for Windows
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
		i. "The science of uncertainty"
			A. extrapolating from samples to populations
			B. Define POPULATION
			C. Define SAMPLE
			D. Give examples (READ ANDREW GELMAN'S BOOK HERE)
				a) Maybe jellybeans? Delicious?
				b) A lesson about bias?
				c) A lesson about extrapolating to unobserved populations
					i. Multiple kinds of jellybeans?
					ii. Or maybe something of different sizes: use a closed scoop to sample. Use only a scoop with big holes to show bias?
				d) How to design experiments and studies to eliminate bias (ensure proper sample to population extrapolation) is the subject of experimental design (different topic)/
				e) Will assume that the experiment has been designed appropriately throughout this course.
		ii. Two goals of statistics:
			A. increase our understanding of the world (hypothesis testing/scientific method)
			B. prediction and forecasting (machine learning/data science)
			C. We will focus on hypothesis testing

2. Basic statistical quantities
	a) How can we characterize the "population" from the "sample"?
	b) Central tendancy: Mean
	c) Spread of individuals: Standard deviation
	d) These quantities are uncertain
		i. An example - Jellybeans again? Have students estimate the mean from different samples
	e) Standard error
	

### Lab Day
1. Introduction to PYSTAN
	a) the blocks
	b) a basic model estimating the mean
		i. A one-sample t-test
		ii. can use this as a basic introduction to statistical inference
			A. point estimates
			B. uncertainty
				A. Tie this into lecture
			C. confidence intervals
			D. adjust sample size and effect size to prove a point about significance
				1. uncertainty goes down as N goes up.
				2. is it more important to be significant, or to know the effect size and uncertainty?
					a) keep this in mind when both writing and reviewing papers
				3. a good for-loop experiment



## Week 3

### Lecture Day

### Lab Day




## Week 4

### Lecture Day

### Lab Day




## Week 5

### Lecture Day

### Lab Day




## Week 6

### Lecture Day

### Lab Day




## Week 7

### Lecture Day

### Lab Day




## Week 8

### Lecture Day

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
