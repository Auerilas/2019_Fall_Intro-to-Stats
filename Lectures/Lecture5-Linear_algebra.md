1. What is linear algebra?
	a. Manipulation of vectors and matrices

	b. Important to know the basic notation and principles
		i. Speeds computation

		ii. Makes code compact

		iii. Can talk generally

		iv. Most good textbooks use linear algebra. Need to know it to read those books

2. Vectors
	a. Notation
		i. Vertical

		ii. Transpose

	b. Addition / subtraction
		i. With scalars

		ii. With other vectors

	c. Multiplication
		i. With scalars

		ii. With other vectors

3. Matrices
	a. Notation
		i. rows x columns

		ii. Transpose

	b. Multiplication
		i. With scalars

		ii. With vectors

		iii. With matrices

		iv. General rule: MxN time NxK = M x K matrix

4. Linear algebra in matrix form
	a. The response is a column vector

	b. Vector of yhats and errors

	c. Decompose the vector of yhats into vector of b0 + b1x1, etc.

	d. Decompose further into a design matrix and vector of coefficients
		i. Step through this VERY slowly and go one line by one line

		ii. Talk about X as the 'design matrix'

	e. Linear algebra notation of regression

5. Transformations
	a. Standardization
		i. How does it work?

		ii. Why do it?
			A. Computational Stability

			B. Interpretation of coefficients in multiple regression (we'll get to this later)

		iii. What does it do to coefficients and interpretation of coefficients?
			A. What does the slope now mean?

			B. What does the intercept now mean?
				1. If only x is standardized?

				2. If both x and y are standardized?

		iv. I generally do this every time

	b. log-y
		i. How does it work?

		ii. Why do it?
			A. Show the equation

			B. Show how it stabilizes variances (they become multiplicative)

			C. It also changes the form (linear to exponential)
				1. We have better ways to stabilize variances that we've already done

				2. I avoid it except in special cases

			D. Useful when data vary over large orders of magnitude (show brain size / body weight example)
