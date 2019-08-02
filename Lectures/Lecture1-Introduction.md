# Lecture 1 - Introduction

1. Who am I?

2. Take a survey
	a. Who has prior stats/programming experience?
	
	b. Even if you do, we will pretend as though no one has any.

3. What is this course?
	a. Will teach the fundamentals of statistics. But it will do so in a thoroughly modern way. It will definitely differ from previous courses or other options here at MU.
		i. We do not talk about null hypothesis testing
			A. Ask students if they know what this is

			B. Give examples: population sizes of animals in urban vs. rural areas, physiological rates change with temperature

			C. Null hypotheses focus on "WHAT", and they are in most cases patently uninteresting and do nothing for science

			D. Good hypotheses instead focus on "how", "when", "where", and perhaps most importantly, "by how much". That is, good hypotheses are carefully thought out and concrete. Students and researchers should spend months on hypotheses before even setting foot in the lab.
	
	b. There will also be no theorems or analytical proofs. This course is focused purely on the application of statistics to help you analyze your data. You will have to learn enough math/background to understand what you are doing.
		i. As a result, this course will be heavily computational, rather than analytical. Using Python and STAN.
	
	c. Will not use the "cookbook" approach
		i. Can show an example of a "statistics flow chart" and discuss why this is a bad idea
	
	d. Instead, will focus on linear models
		i. Refer back to the flowchart. Every test here can be formulated as a linear model, so linear models are incredibly flexible.

	e. We can't cover it all. We will cover the basics to give you a good sense of most of the analyses you'll have to do. But we will go "slow". I'd rather you have a deep understanding of a few topics, which you can use to learn more on your own, rather than no understanding of many topics.

4. Materials
	a. No required textbooks
		i. There are recommended books:
			A. Quinn and Keough - Experimental Design
	
			B. Ramsey and Schaffer - Statistical Sleuth
	
			C. Draper and Smith - Applied Regression
	
			D. Gelman and Hill - Multilevel models

	b. You will HAVE to have a laptop (department will provide if needed)

5. Class format
	a. One lecture per week (one hour)
		i. No powerpoints. Plenty of research suggests that powerpoints are bad for learning. Plus, writing by hand forces ME to slow down too, and forces you to take notes. So everybody goes slower, which is good.

	b. One computer lab per week (two hours)
		i. Hands on practice with programming and stats
	
		ii. Will also cover new material because one lecture just isn't enough. This means that some learning will occur on your own through the lab (though I am happy to help).
	
		iii. There will be a LOT of repitition, both because the material demands it and by design to help you learn.

6. Grading
	a. No tests or memorization (I don't want to test how well you memorize something. I'd rather you learn it)

	b. The key to learning is practice, practice, practice.
		i. Weekly lab exercises (given on lab day, to be turned in the following class)
			A. These will be detailed and long (and might include new material)
	
			B. These will be started during the "lab" class, so I'll be around for two hours to help.
	
			C. Can also come to me during office hours (by appointment)
	
			D. Distributed via github. Turn in to me digitally.
		ii. Weekly quizzes
			A. Short. One or two detailed analysis questions. Only on previous material (no new stuff)
	
			B. Turned in digitally

	c. By necessity, stats are cumulative. You must show up every week and do the work every week, because each week builds on the last. I won't take role, nor am I responsible if you miss classes. If you have to miss more a legitmate reason, please let me know. But you will ultimately be responsible for the material.

	d. Final project
		i. Analyze real data to answer real questions
			A. Can use your own, but talk to me first
	
			B. I'll provide data for those who don't have it

7. Get Anaconda set up (I should print out detailed instructions for all operating systems)
	a. Download and install Anaconda
		i. Hit yes on path modification
	
		ii. Run 'python' from the Terminal, check Anaconda
	
		iii. Set up conda forge
	
		iv. Update all packages
	
		v. Install pystan

