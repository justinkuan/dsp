[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

> **Exercise 4**   Using the variable *totalwgt_lb*, investigate whether first babies are lighter or heavier than others. Compute Cohen’s d to quantify the difference between the groups. How does it compare to the difference in pregnancy length?  

> Results:  
> Cohen's D for pregnancy length is **0.029** standard deviations  
> Cohen's D for birth weight standard deviations **-0.089** standard deviation  
> We find that effect of first babies on birthweight is similar to its effect on pregnancy length, small and almost negligible.

> Code:
~~~~
live = preg[preg.outcome == 1]
firsts = live[live.birthord == 1]
others = live[live.birthord != 1]
CohenEffectSize(firsts.prglngth, others.prglngth)
CohenEffectSize(firsts.totalwgt_lb, others.totalwgt_lb)
~~~~
