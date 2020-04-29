# Neurotech Final Assignment
**"In case of stats, break into this file"**

Create a document for your future self, which details how to approach a data analysis problem.

Link to assignment: https://docs.google.com/document/d/16sKhxWau2iDriuojcPUmc3H_BwefQaHKv2BSkZfNlkY/edit#heading=h.7n2qer5ew2y7

### Some basic probability terms and concepts
- Conditional probability P(A|B) = P(A∩B)/P(B)
- Bayes rule: P(B|A) = (P(A|B) * P(A))/P(B)
- Why are outliers important?
  *  Outliers will skew the mean and increase the standard deviation of a   dataset. However, outliers don’t affect the median or mode very much.
- How to represent data:
  * [Probability mass function](https://en.wikipedia.org/wiki/Probability_mass_function): gives the probability that a discrete variable is exactly equal to some value x
  * [Probability density function](https://en.wikipedia.org/wiki/Probability_density_function): gives the probability that a continuous variable is exactly equal to some value x
  * [Cumulative distribution function](https://en.wikipedia.org/wiki/Cumulative_distribution_function): gives the probability that a continuous or discrete variable is less than or equal to some value x
- P-values: P value represents the probability that a result this extreme or more extreme would happen by random chance if the null hypothesis is true. In science, a P-value of 0.05 is often used to determine whether results are statistically significant.
- Effect size vs. Statistical Significance
  * Statistical Significance: A statistically significant result means that the results OR more extreme results are unlikely if the null hypothesis is true (usually means they have less than 5% chance of happening by chance). Statistical significance is useful for determining if the results mean that you can fail to reject the null hypothesis or not.
  * Effect size is the size difference between groups in terms of the standard deviation, and can often be calculated by (mean(A) - mean(B))/Standard deviation. Effect size is useful for figuring out how big the difference between two groups is.
  * A study with a small sample size might show a large effect size, but not be statistically significant, and a study with a large sample size but very small differences between the groups might show a small effect size, but be statistically significant.
- False Positives vs. False Negatives
  * A false positive, or type 1 error is when a test comes back positive when the true result is negative
  * A false negative, or type 2 error, is when a test comes back negative when the true result is positive
  * When testing for a rare disease among many people who are unlikely to have it, the number of false positives can be surprisingly high. This is due to the fact that there are many more people who have the disease than who don't have the disease. In other words, the P(actual=0 | screen=1) for the general population can actually often be higher than P(actual=1 | screen=1). See the week 2 assignment for more details, and an example.

### How to test a hypothesis
Based on this:
https://docs.google.com/document/d/1un3ktVI5TszrWPqvOtlkFC-b8ghoYDOqR86uorV5A_Y/edit

What is hypothesis testing, and why would I want to do it?

A hypothesis test will evaluate how likely the null hypothesis (nothing interesting is happening, there is no effect behind the data) is to occur given the data, P(Null Hypothesis | Data). When you have completed your hypothesis test, you will know whether you should reject or fail to reject your null hypothesis. This is important, because it will tell you if your results are statistically significant.

1. Plot the data, understand the data, know the data
  - Maybe take the mean, median, and standard deviation of the data
  - If applicable, read the scientific article that the data came from, and make sure you understand what was done to get the data, and if any preprocessing has already been done
2. Check for missing data, and remove missing data points as necessary, or determine another way to deal with them (substitute in the mean?)
3. Define the problem. What exactly is the question that you are trying to answer?
  - Make sure the data is in the correct format to answer the question. Maybe you need to do some preprocessing to make the data more useful
4. Figure out which test to perform
  - Here is a helpful and simple flow chart to figure out which test to perform:
  <html>
  <img src="https://github.com/katie608/neurotech/blob/master/finalResources/TandZflowchart.png" width="300" height="auto" />  </html>
  - There are also more complete flowcharts and a description of the tests in the Final Resources folder
  - Make sure that your dataset fulfills all the assumptions that the test requires. For example, some tests may require that your data is normal. If your data is not normal, you might want to look into a bootstrapping approach, which relies on the central limit theorem.
5. Perform the test
  - Matlab has a command for about every test. [Scipy](https://docs.scipy.org/doc/scipy/reference/stats.html) also has many built in statistical tests.
6. Interpret the results
  - State whether the null hypothesis was accepted or rejected
  - Make a graph, and use the graph to do the "does this make sense" test

For an example of hypothesis testing in Matlab, see week 4 assignment.
