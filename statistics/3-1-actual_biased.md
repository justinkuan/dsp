[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

> **Exercise 1**   Something like the class size paradox appears if you survey children and ask how many children are in their family. Families with many children are more likely to appear in your sample, and families with no children have no chance to be in the sample.  
> Use the NSFG respondent variable NUMKDHH to construct the actual distribution for the number of children under 18 in the household.  

> Now compute the biased distribution we would see if we surveyed the children and asked them how many children under 18 (including themselves) are in their household.

> Plot the actual and biased distributions, and compute their means. As a starting place, you can use chap03ex.ipynb.

>> Actual mean of 1.024205155043831  
>> Biased mean of 2.40367910064282  

>> plot will be added later, code for plot is included below.

~~~~
# Exercise 3.1
pmf_nsfg = thinkstats2.Pmf(f.numkdhh , label='observed')
biased_pmf_nsfg = BiasPmf(pmf_nsfg , label='actual')

thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf_nsfg, biased_pmf_nsfg])
thinkplot.Show(xlabel='number of children', ylabel='PMF')
~~~~
