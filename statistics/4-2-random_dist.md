[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

> **Exercise 2**   The numbers generated by random.random are supposed to be uniform between 0 and 1; that is, every value in the range should have the same probability.
>Generate 1000 numbers from random.random and plot their PMF and CDF. Is the distribution uniform?  

>> Looks good.  The PMF & CDF approximates nearly identically to the PMF & CDF of a uniform distribution.  

~~~~
# Exercise 4.2
random_test = np.random.random(1000)

# PMF & CDF
random_pmf = thinkstats2.Pmf(random_test)
thinkplot.SubPlot(1)
thinkplot.Pmf(random_pmf)
thinkplot.Config(xlabel='Random Draw', ylabel='PMF')

random_cdf = thinkstats2.Cdf(random_test)
thinkplot.SubPlot(2)
thinkplot.Cdf(random_cdf)
thinkplot.Config(xlabel='Random Draw', ylabel='CDF')
~~~~
