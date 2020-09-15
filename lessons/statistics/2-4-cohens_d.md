[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

 
```
firsts_weight = firsts.totalwgt_lb.mean()  
others_weight = others.totalwgt_lb.mean()  
print('firsts mean weight = ', firsts_weight)  
print('others mean weight = ', others_weight)  
```

>firsts mean weight =  7.201094430437772  
>others mean weight =  7.325855614973262  


```
cohens_d_weight = CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)  
cohens_d_length = CohenEffectSize(firsts.prglngth, others.prglngth)  
print('Cohens\'s d for weight = ', cohens_d_weight)  
print('Cohens\'s d for pregnancy length = ', cohens_d_length)  
```

>Cohens's d for weight =  -0.088672927072602  
>Cohens's d for pregnancy length =  0.028879044654449883  

The first thing I noticed was that Cohen's d for weight is a negative value. Based on the formula for Cohen's d, that simply means that the mean for the first group is smaller than the mean for the second group. If I were to switch the order of the inputs, I would get the same value just positive.

When comparing the absolute value of Cohen's d for both weight and length of pregnancy, the one for weight is slightly larger but it does not seem to be by a significant factor. I do not believe there is a significant difference in weight or duration of pregnancy between a first child and the others.