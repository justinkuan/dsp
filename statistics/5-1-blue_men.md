[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> About 34.275% of the US male population is between 5'10 and 6'1.  

~~~~
# Exercise 5.1
# Creating our normal distribution using BRFSS
mean = 178
sd = 7.7
dist = scipy.stats.norm(loc=mean, scale=sd)

# ppl between 5'10" and 6'1" is simply the difference in cdf of the two
# conversion 2.54 cm to 1 inch
# 5'10 = 70 inches
# 6'1 = 73 inches
a = dist.cdf(70*2.54)
b = dist.cdf(73*2.54)
print(f'About {round((b-a)*100, 3)}% of the U.S. male population is in this range.')
~~~~
