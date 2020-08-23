# Bayesian A/B testing

The Bayesian approach is a very intuitive way to do A/B testing. Unlike the frequentist approach, it does not include hypothesis testings, Z-scores, X<sup>2</sup> scores, or p-values

There are many advantages to doing it this way. <br>
Advantages include:
- interpretability
- (sample) size doesn't matter
- allows more flexibility
- end result is a probability distribution, rather than a point estimate. 
Instead of having to think in terms of p-values, we can think directly in terms of the distribution of possible effects of our treatment. This makes it much easier to understand and communicate the results of the analysis
- compute more understandable quantities about our uncertainty

Although there is no free lunch, there are many great reasons to use this intuitive technique. 
And it just means there is more than one way to solve a problem.

## The Bayesian approach 
The Bayesian approach goes something like this:

1. Define the prior distribution that incorporates your subjective beliefs about a parameter. The prior can be uninformative or informative.
2. Gather data.
3. Update your prior distribution with the data using Bayes’ theorem (though you can have Bayesian methods without explicit use of Bayes’ rule—see non-parametric Bayesian) to obtain a posterior distribution. The posterior distribution is a probability distribution that represents your updated beliefs about the parameter after having seen the data.
4. Analyze the posterior distribution and summarize it (mean, median, sd, quantiles…).
