Module 5 – Probability: Explanations

#1. Basics of Probability

#a.Tossing a Coin 10,000 Times

We simulate tossing a fair coin 10,000 times using `random.choice(['H', 'T'])`. We count how many times it lands on heads or tails, and calculate the probability of each outcome by dividing the count by the total number of tosses.

#b. Rolling Two Dice and Getting a Sum of 7

We simulate rolling two six-sided dice 10,000 times using `random.randint(1, 6)`. We check how many times the sum of the two dice is 7 and estimate the probability by dividing this count by the total trials.

#2. At Least One "6" in 10 Rolls

We estimate the probability of getting at least one '6' in 10 rolls of a fair die. For each trial, we roll the die 10 times and check if any of them is a 6. We repeat this process many times and calculate the proportion of successful trials (those with at least one 6).
#3. Conditional Probability and Bayes' Theorem

#a. P(Red | Previous was Blue)

We simulate drawing a ball (red, green, or blue) 1000 times with replacement from a bag. We track sequences of draws to estimate the probability that a red ball is drawn given that the previous draw was blue.

#b. Verify Bayes' Theorem

We use the same simulated data to verify Bayes’ theorem:
P(R|B) = \frac{P(B|R) \cdot P(R)}{P(B)}

We compute each term using counts from the simulated transitions and compare the result with the direct conditional probability.

#4. Discrete Random Variable

We generate a random sample of size 1000 using `np.random.choice()` from a discrete distribution where:
P(X=1) = 0.25
P(X=2) = 0.35
P(X=3) = 0.40

We calculate the empirical mean, variance, and standard deviation using `numpy` functions to summarize the sample's behavior.

#5. Continuous Random Variable – Exponential Distribution

We simulate 2000 samples from an exponential distribution with a **mean of 5** using `np.random.exponential()`. We then visualize the data:
As a histogram of the sample
With a PDF (Probability Density Function)** overlay using `scipy.stats.expon`

This shows how well the data matches the theoretical exponential shape.

#6. Central Limit Theorem (CLT)

We demonstrate the Central Limit Theorem by:
Generating 10,000 values from a **uniform distribution**.
Taking 1000 random samples of size 30 and computing their means.
Plotting:
The original uniform distribution
The distribution of sample means

The result shows that the distribution of the sample means is approximately normal, even though the original data is **uniform**—this is the essence of the Central Limit Theorem.
