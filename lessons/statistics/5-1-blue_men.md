[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

```
import scipy.stats

mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)

#cdf(6'1") - cdf(5'10")
dist.cdf(185.42) - dist.cdf(177.8)
```
> **0.3427468376314737**

About 34% of men are between 5'10 and 6'1"