# Neurotech Final Assignment
**"In case of stats, break into this file"**

Create a document for your future self, which details how to approach a data analysis problem.

Link to assignment: https://docs.google.com/document/d/16sKhxWau2iDriuojcPUmc3H_BwefQaHKv2BSkZfNlkY/edit#heading=h.7n2qer5ew2y7

### Some basic probability terms and concepts
- Conditional probability P(A|B) = P(A∩B)/P(B)
- Bayes rule: P(B|A) = (P(A|B) * P(A))/P(B)
- Why are outliers important?
Outliers will skew the mean and increase the standard deviation of a dataset. However, outliers don’t affect the median or mode very much.
- P-values: P value represents the probability that a result this extreme or more extreme would happen by random chance if the null hypothesis is true. In science, a P-value of 0.05 is often used to determine whether results are statistically significant.
- Statistical Significance: A statistically significant result means that the results OR more extreme results are unlikely if the null hypothesis is true (usually means they have less than 5% chance of happening by chance). Statistical significance is useful for determining if the results mean that you can fail to reject the null hypothesis or not. 
- Effect size is the size difference between groups in terms of the standard deviation, and can often be calculated by (mean(A) - mean(B))/Standard deviation. Effect size is useful for figuring out how big the difference between two groups is.
- A study with a small sample size might show a large effect size, but not be statistically significant, and a study with a large sample size but very small differences between the groups might show a small effect size, but be statistically significant.
- False positive vs False negative, and the sort of paradox about them (see week 2 for more details)

### How to test a hypothesis
Based on this:
https://docs.google.com/document/d/1un3ktVI5TszrWPqvOtlkFC-b8ghoYDOqR86uorV5A_Y/edit
1. Plot the data, understand the data, know the data
2. Check for missing data, and remove missing data points as necessary, or determine another way to deal with them (substitute in the mean?)
3. Define the problem. What exactly is the question that you are trying to answer?
4. Figure out which test to perform
5. Perform the test
6. Interpret the results: make a graph, write whether or not the null hypothesis was accepted or rejected

### How to do Machine learning in Matlab
(If I get to this, might be good information to remember, since matlab's classification learner tool lets you easily and quickly run a lot of different models on the data, which is helpful for figuring out which type of model might work the best)
